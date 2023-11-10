### 若你已经修改了部分文件、并且将其中的一部分加入了暂存区，应该如何回退这些修改，恢复到修改前最后一次提交的状态？给出至少两种不同的方式

1.回退到最后一次提交的状态并清除暂存区中的所有更改，可以使用以下命令: `git reset --hard HEAD`

这将取消所有的更改并回到最后一次提交的状态。

2.取消某个特定文件的更改，可以使用以下命令: `git checkout -- filename`



### 若你已经提交了一个新版本，需要回退该版本，应该如何操作？分别给出不修改历史或修改历史的至少两种不同的方式

> ##### 不修改历史的
>

1.用`git log`命令查看提交历史，找到哈希值（commit hash）

2.使用命令：`git reset --hard commit_hash`来回退到特定的提交

> ##### 修改历史的

   1.使用 `git log` 命令查找你要回退的提交的哈希值

2. `git branch backup_branch`来保存已有的工作
3. 使用 `git reset` 命令来回退到你想要的提交：`git reset --hard commit_hash`
4. 使用以下命令来强制推送：`git push -f origin your_branch_name`



### 我们已经知道了合并分支可以使用 merge，但这不是唯一的方法，给出至少两种不同的合并分支的方式

除了`merge`来合并分支，还可以使用 `rebase` 和 `cherry-pick`

`rebase`（变基）的合并分支命令为

```sh
git checkout feature-branch
git rebase main
```

而`cherry-pick`（摘取）的合并分支命令为`git cherry-pick commit_hash`

因此我们在cherry-pick前先要找到提交的哈希值