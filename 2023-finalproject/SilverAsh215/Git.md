# First question

## 1.restore

git restore --staged <file_name> : 将暂存区中的文件移出

![restore](photo/restore.png)

git checkout -- <file_name> : 当文件被移出暂存区后，可将本地文件还原为远程仓库中的文件

## 2.reset

git reset HEAD <file_name> : 重置

![reset](photo/reset.png)

git checkout -- <file_name> : 当文件被移出暂存区后，可将本地文件还原为远程仓库中的文件

# Second question

## 1.reset --hard

git reset --hard <版本号> : 回退版本，删除历史，修改本地仓库

![reset --hard](photo/reset%20---hard.png)

## 2.reset

git reset <版本号> : 回退版本，删除历史，不修改本地仓库

![process](photo/process.png)

## 3.revert

git revert -n <版本号> : 重做版本，增加历史

![revert](photo/revert.png)

# Third question

## 1.rebase

git rebase  <branch>

![rebase](photo/rebase.png)

## 2.cherry-pick

git cherry-pick <版本号>

![cherry-pick](photo/cherry-pick.png)
