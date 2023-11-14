# Git answer

## by 陈欢

### Q1：若你已经修改了部分文件、并且将其中的一部分加入了暂存区，应该如何回退这些修改，恢复到修改前最后一次提交的状态？给出至少两种不同的方式

#### A1：

1.使用 `git reset`回退到最近一次提交的状态

`git reset`：将暂存区的更改**全部**撤销，并将其重置到上次提交的状态。

`git reset <file>`：将**指定文件**的更改撤销，并将其重置到上次提交的状态。
![git reset](./picture/git%20reset.png)

2.使用 `git rm --cached`回退到最近一次提交的状态

![git rm](./picture/git%20rm.png)

---

### Q2:若你已经提交了一个新版本，需要回退该版本，应该如何操作？分别给出不修改历史或修改历史的至少两种不同的方式

#### A2：

1.使用 `git revert`此种方法不会修改历史。

`git revert <commit-hash>`：创建一个新的提交，这个新提交是对你想要回退的提交的逆操作。这样做不会改变历史。
你需要替换`<commit-hash>`为你**想要回退**的提交的哈希值:
用`git log`查看提交历史，找到哈希值
![git revert](./picture/git%20revert.png)

2.使用 `git reset --hard`此种方法会修改历史。

`git reset --hard <commit-hash>`：将当前分支重置为`<commit-hash>`版本，并删除所有未提交的更改和暂存。
注意此处，你需要替换`<commit-hash>`为你**想要回退至**的提交的哈希值（并不会回退此版本）

![git reset --hard](./picture/git%20reset%20--hard.png)

---

### Q3：我们已经知道了合并分支可以使用 merge，但这不是唯一的方法，给出至少两种不同的合并分支的方式

#### A3：

1.使用 `git merge`

`git merge <branch-name>`：将`<branch-name>`分支合并到当前分支。

![git merge](./picture/git%20merge.png)

2.使用 `git rebase`

`git rebase <branch-name>`：将`<branch-name>`分支合并到当前分支。这个过程是通过临时**移除**一系列的提交（即当前分支上的提交），然后在目标分支的最新提交之后，再逐一**应用**这些提交。

![git rebase](./picture/git%20rebase.png)


###### end~~~

---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
###### 呜呜呜