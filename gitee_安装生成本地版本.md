#### 1.注册gitee以及安装git shell

首先注册gitee并安装好gitshell

#### 2.进行公钥的设置

git shell 安装好之后,打开git bash

输入 ssh-keygen -t rsa -C "用户名"  之后连续两次回车

之后在C盘用户目录下的.ssh中找到id_rsa.pub并复制其中的内容

然后点开码云上的设置

点击ssh公钥

将刚才得到的密钥复制进公钥输入框即可

#### 3.gitee上创建好仓库

#### 4.本地创建一个文件夹作为本地仓库，

```
# 克隆下你刚建立的仓库地址
git clone 仓库地址
建立仓库
git init 
```

#### 5.将项目拷贝到当前仓库

#### 6.将项目上传到本地git缓存

```
方法一 git add 添加多个文件，文件之间以空格隔开
git add file1 file2 file3 
方法二 多次git add
git add file1
git add file2
git add file3
方法三 添加指定目录下的文件
config目录下及子目录下所有文件，home目录下的所有.php文件
git config/*
git home/*.php
方法四 git add . 添加所有的文件， 或者 git add --all 添加所有的文件
git add .
git add --all
git add 文件夹
git add 文件夹名
```

#### 6. 添加批注

```
git commit -m "add new file"
```

#### 7.推送到远端仓库

```
git push origin master
第一次需要使用下面的命令
git push -u origin master
```

#### .. 

1. 创建空目录

```

$ mkdir learngit
$ cd learngit
$ pwd
/Users/michael/learngit
```

2. 进入创建的目录，初始化git仓库
```
git init
```

3. 把文件添加到版本库

```
git add readme.txt
git commit -m "批注"
```

4. 在本地的`learngit`仓库下运行命令

```
git remote add origin git@github.com:用户名/仓库名.git
```

5. 把本地库的所有内容推送到远程库上

> 把本地库的内容推送到远程，用`git push`命令，实际上是把当前分支`master`推送到远程。
>
> 由于远程库是空的，我们第一次推送`master`分支时，加上了`-u`参数，Git不但会把本地的`master`分支内容推送的远程新的`master`分支，还会把本地的`master`分支和远程的`master`分支关联起来，在以后的推送或者拉取时就可以简化命令。

```
git push -u origin master
git push origin master
```

6. 删除远程库

```
git remote -v
根据名字删除，比如删除origin:
git remote rm origin
```












