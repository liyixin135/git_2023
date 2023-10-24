# Git的学习笔记

git分为工作区（workspace）、缓存区（index）、本地仓库（repository）以及远程仓库（remote）

workspace为当前工作目录，git add 后文件进入缓存区，位于.git的index文件中。

**git 常见命令：**

git init   

git status  查看当前仓库情况

git add   添加到缓存区

git commit  -m “对新版本做出的修改做出简单的描述”提交到本地仓库

（要求为1首字母大写，2英文描述，3要有句号。）

git log 查看版本情况

git reset --hard 要回滚版本序号

**创建新分支**

git branch 分支名

**切换分支**

git checkout 分支名

**创建并切换新分支**

git checkout -b 分支名

**保存当前工作且切换分支**

git stash

**切换会原来的分支，并状态恢复**

git stash pop

**github克隆仓库**

git clone [url]

## 学习总结

在这次git工具的学习中，我明白了一个团队是如何做到多人同时维护修改一个项目并将其进行整合。

在这过程中我学到了git的基本使用命令和如何从github上拉取他人项目并提交pr，让我对多人项目开发协作有了更深的了解。