sudo apt install git

git config --global user.name "你的github用户名"

git config --global user.email "你github注册时使用的邮箱"

#### [<1>创建本地空仓库](https://github.com/liyixin135/teach/blob/main/git.md#1创建本地空仓库)

```
mkdir test
cd test
git init
```

git status

备注：status查看当前仓库状态

cd test
touch test.md
git status
git add test.md
git status
git commit -m "Add new file."

add:将文件添加到缓存区

commit：提交到本地仓库

git add --all

git commit --amend

git log

git reflog

git reset --hard 要回滚版本

git reset --hard HEAD^

git reset --hard HEAD~3

创建新分支

```
git branch 分支名
```

​    

备注：可用git branch查看分支
 切换分支

```
git checkout 分支名
```

​    

创建并切换新分支

```
git checkout -b 分支名
```

注意事项：若切换分支前，所在分支存在未commit的内容，会把这部分未commit内容连带到所切分支上

##### [解决方案，保存当前工作切换分支：](https://github.com/liyixin135/teach/blob/main/git.md#解决方案保存当前工作切换分支)

```
git stash
```

​    

此时就不需要担心未commit内容连带到所切分支上 查看当前存储了多少工作状态

```
git stash list
```

​    

切换会原来的分支，将状态恢复

```
git stash pop
```

git clone [url]













# git应用

