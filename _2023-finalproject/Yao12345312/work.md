#### 回退暂存区文件到修改前最后一次提交的状态
- `git reset <file>`

 可加`--mixed`回退到本地并且不影响工作区内容
- `git checkout <file>`
#### 回退已经提交的版本
- 需要修改历史时，可用`git reset HEAD^`来回退到上个版本。在`git push -f`后，它之后的修改历史会消失


- 如果不需要修改历史，可用`git revert --no-commit <commit>..HEAD `命令。它将撤销<commit>到HEAD期间的所有更改，并创建一个新的提交来存储这些变更,`commit`到`HEAD`期间的更改都会被保留。

#### 合并分支
###### 需要注意在合并前应该先切换到目标分支，如果为多人项目的话还应`git pull`保证分支为最新状态
- 如果需要合并某个分支上的单个commit，可用`git cherry-pick <commit>`，这样`commit`就被合并，不过有可能会合并冲突，此时需要手动添加`commit`

- 可通过`git rebase`命令来进行合并分支，注意已经推送到远程的内容就不要变基，有可能会产生冲突，这时需要手动解决冲突后用`git status` `git rebase --continue`来继续操作

- 如果不想通过输入指令来合并，可以通过开发工具`IDEA`
来进行分支代码合并

![rm](/home/huangjunyao/git_2023/_2023-finalproject/Yao12345312/1.jpeg)
