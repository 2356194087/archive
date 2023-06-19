#  git 文档

## 初始化
#### 初始化git项目
~~~ powershell 
 $ mkdir dome  
 $ cd dome
 $ git init 
~~~

## git配置
#### 设置git用户名  邮箱
~~~ powershell 
 $ git config user.name xxxxx 
 $ git config user.email 22286654@qq.com
~~~

## git 文件操作
#### 1、添加文件到缓存区 ( . 或 * 代表全部)
~~~ powershell 
 $ git add lianxi.txt 
 $ git add .
 $ git add *
~~~

#### 2、将 git add 暂存的文件 提交到本机git仓库
~~~ powershell 
 $ git commit -m "提交说明"
~~~

#### 3、查看当前git提交状态
~~~ powershell 
 $ git status
~~~ 

#### 4、git 版本 退回 
~~~ powershell 
 $ git reset  --hard Head~0   //回退到上次提交的版本 
 $ git reset --hard [版本号]  //回退指定版本
~~~ 

#### 5、git 状态 退回 
~~~ powershell 
git reset HEAD [文件或文件目录]  // 将文件从缓存区退回到编辑区
git checkout -- [文件或文件目录] // 将文件退回到没有修改前
git restore [文件或文件目录]     // 将文件退回到没有修改前
~~~ 

## git 分支

#### 查看当前分支
~~~ powershell 
$ git branch 
~~~

#### 创建分支 ( git 默认 有一个 ***master*** 分支 )
~~~ powershell 
$ git branch dev // 创建一个dev分支
~~~

#### 切换分支 
~~~ powershell 
$ git checkout dev // 切换到dev分支
~~~

## git 记录日志
#### 查看日志
~~~ powershell 
$ git reflog  // 查看所有提交的版本号
$ git log     // 查看历史日志 
$ git log --oneline    // 查看简洁版日志
~~~