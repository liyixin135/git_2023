> 要求： 编写一个文档，回答下列问题，这些问题的答案都应当使用 git 命令实现
> 提交： 一个 MarkDown 文件和若干个图片文件，在 MarkDown 中使用有效的相对路径引用你的图片
>
> 1.若你已经修改了部分文件、并且将其中的一部分加入了暂存区，应该如何回退这些修改，恢复到修改前最后一次提交的状态？
>
> 2.给出至少两种不同的方式 若你已经提交了一个新版本，需要回退该版本，应该如何操作？分别给出不修改历史或修改历史的至少两种不同的方式&#x20;
>
> 3.我们已经知道了合并分支可以使用 merge，但这不是唯一的方法，给出至少两种不同的合并分支的方式

# 问题一

## 方法一：使用 git restore 命令

首先，使用 git status 命令查看暂存区和工作区的状态，确认哪些文件被修改但未加入暂存区。
使用 git restore --staged <文件路径> 命令将暂存区中的指定文件回退到最后一次提交的状态，文件路径可以是单个文件或者文件夹。
如果需要同时撤销工作区中对应文件的修改，可以使用 git restore <文件路径> 命令。这将会将工作区中的文件回退到最后一次提交的状态。

![1\_1.jpg](https://note.youdao.com/yws/res/363/WEBRESOURCEf6092a56453c3eb3e359e30b534e53b0)

## 方法二：使用 git checkout 命令

使用 git checkout -- <文件路径> 命令将工作区中的指定文件回退到最后一次提交的状态。
如果要将暂存区中的文件回退到最后一次提交的状态，可以先执行 git restore --staged <文件路径> 命令，然后再执行 git checkout -- <文件路径> 命令。

![1\_2.jpg](https://note.youdao.com/yws/res/366/WEBRESOURCE9bc73eaea92eebed18446f5928592b18)

# 问题二

## 不修改历史：1. 使用git revert命令：

这个命令会创建一个新的提交，将指定的提交的更改撤销，并将撤销的更改添加到代码库中。

![2\_1.jpg](https://note.youdao.com/yws/res/369/WEBRESOURCE03dd7b2eec5d3038536db0aca1f7dd71)

## 修改历史：1.  使用git reset命令：

这个方法可以用来回退到任何一个历史提交并且将HEAD指向该提交。

![2\_2\_1.jpg](https://note.youdao.com/yws/res/371/WEBRESOURCEccae6d0e9125d7bd55a517300ac0995e)

## 2.使用git cherry-pick命令：

这个命令可以选择性地将一个或多个提交从一个分支复制到另一个分支。首先，找到你想要回退的提交的SHA标识符。然后，在你的分支上运行，然后将目标提交复制到当前分支，实现回退的效果。

![2\_2\_2.jpg](https://note.youdao.com/yws/res/373/WEBRESOURCEedf17f9773ac68344395c6e16133c3c9)

# 问题三

## Rebase：

这是将一个分支的提交放置在另一个分支的最新提交之后。可以创建一个更整洁、线性的提交历史。使用`rebase`命令可以将当前分支的提交移动到目标分支的顶部，使得当前分支的提交看起来是基于目标分支最新提交的。

![3\_2\_1.jpg](https://note.youdao.com/yws/res/379/WEBRESOURCE25d18cf9e1113e961fbf1f03935f9392)

![3\_1\_2.jpg](https://note.youdao.com/yws/res/381/WEBRESOURCE3e956e754fc6da8ea7c21a0f9d4c299d)



## Cherry-pick：

Cherry-pick 可以选择某个分支上的一个或多个提交，并将它们应用到当前分支上。这种方法可以选择性地合并特定的提交，而不是一次性合并整个分支。

![3\_2\_1.jpg](https://note.youdao.com/yws/res/383/WEBRESOURCE9e13a4946f7065ca5716fc71d20e6e4a)![3\_2\_2.jpg](https://note.youdao.com/yws/res/385/WEBRESOURCEa864ca925c738292167f2d5734aaa18f)![3\_2\_3.jpg](https://note.youdao.com/yws/res/387/WEBRESOURCEe31fcde93c0bcc48425a48a5d4ea7b74)

