# 一些总结和心得

## by 陈欢

参加DynamicX培训，其中很重要的一环就是学习Git的使用。从中，我学习到了Git的优势和具体使用方法，了解了Git的常用命令，提高了我的工作效率。在学习过程中，我的进步离不开DX团队学长学姐的帮助，在我培训遇到困难时给予技术支持与帮助，同时在大学生活和学习中也给我答疑解惑，扫清迷雾，指明了方向，由衷地对DX的学长学姐们表示感谢！（呜呜呜李奕欣学姐，人美心善，她真的，我哭死！）

### 1.Git是什么？

Git是一款开源的分布式版本控制系统，用于敏捷高效地处理任何或小或大的项目。Git是Linus Torvalds为了开发Linux内核而开发的一个开放源码的版本控制软件。Git与SVN类似，但Git采用了分布式版本库的方式，不需要服务器端软件支持。

### 2.Git的安装

    在Linux上安装Git，只需要打开终端，输入
    
    $ sudo apt-get install git
    
    即可。

### 3.Git的使用

#### 3.1 创建版本库

    在本地创建一个空目录，在终端中进入该目录，输入
    
    $ git init
    即可创建一个版本库。

#### 3.2 配置Git

    在终端中进入版本库，输入
    
    $ git config --global user.name <username>
    $ git config --global user.email <email>
    即可配置用户名和邮箱。

#### 3.3 添加文件

    在版本库中添加文件，需要先将文件添加到暂存区，再提交到版本库。
    
    在终端中进入版本库，输入
    
    $ git add <file>
    
    将文件添加到暂存区。
    
    $ git commit -m "commit message"
    将文件提交到版本库。

#### 3.4 版本回退

    在版本库中，可以对文件进行多次修改，并提交到版本库。
    
    在终端中进入版本库，输入
    
    $ git log
    
    查看提交历史。
    
    $ git reset --hard HEAD^
    
    回退到上一个版本。
    
    $ git reset --hard HEAD~2
    
    回退到前两个版本。

#### 3.5 分支管理

    在终端中进入版本库，输入
    
    $ git branch
    查看分支。
    
    $ git branch <branch name>
    创建分支。
    
    $ git checkout <branch name>
    切换分支。
    
    $ git merge <branch name>
    合并分支。
    
    $ git branch -d <branch name>
    删除分支。

#### 3.6 仓库克隆

    在终端中进入版本库，输入
    
    $ git clone <url>
    即可克隆一个版本库。

#### 3.7 远程仓库

    在版本库中，可以提交到远程仓库。
    
    在终端中进入版本库，输入
    
    $ git remote add origin <url>
    即可添加远程仓库。
    
    $ git push -u origin master
    将本地版本库的master分支推送到远程仓库。
    
    $ git push origin master
    将本地版本库的master分支推送到远程仓库。
    
    $ git pull
    将远程仓库的master分支拉取到本地。
    
    $ git fetch origin master
    将远程仓库的master分支拉取到本地，不合并到当前分支。
