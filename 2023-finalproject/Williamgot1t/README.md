# README

在这个git学习的课程中 我收益匪浅 从中有着巨大的收获

### 使用Github的原因

使用github而不是gitee 因为github中有着来自全世界的优秀代码将来对内的许多代码也需要从中获取 因此 这是一个必要的学习内容

并且 在全英的环境中操作 更能提高自己的工作能力 能使未来的工作更加得心应手

### Git的一些操作

文件状态：是否修改；是否跟踪；是否提交

- git add<>  将文件提交即跟踪

- git commit -m<>将文件提交

- git rm 将文件删除

- git reset head~--soft<> 撤销提交（第一次不可）

- git status    查看文件状态

- git diff   查看文件具体哪里修改

- git log 查看历史提交记录


可美化输出形式

- git log pretty=**

如：oneline  graph

- $git log --pretty=format:"%h-%an,%ar:%s"

%h 美化哈希值

%an  作者名字

%ar  修订日期（至今）

% ad 修订日期

%s  提交说明

**git branch** + 分支名

**git checkout**  + 分支名 切换到分支

（现在可能更常用 git switch）

git checkout -b +分支名 可以直接创建并切换到新分支

**git stash**（用来保存当前工作）

- git stash save 注释

  作用等同于git stash，区别是可以加一些注释， 执行存储时，添加注释，方便查找

- git stash pop

  默认恢复git栈中最新的一个stash@num，建议在git栈中只有一条的时候使用，以免混乱注:该命令将堆栈中最新保存的内容删除

- git stash list

  查看当前stash的所有内容

- git stash apply

  将堆栈中的内容恢复到当前分支下。这个命令不同于 git stash pop。该命令不会将内容从对堆栈中删除，也就是该命令能够将堆栈的内容多次运用到工作目录，适合用与多个分支的场景

- git stash drop从堆栈中移除指定的stash

  使用方法: git stash drop stash@$num]

- git stash clear

  移除全部的stash

- git stash show

  查看堆栈中最新保存的stash和当前目录的差异，显示做了哪些改动，默认show第一个存储

### 一些感悟

在使用ubuntu的linux系统中 许多与git操作有着相似之处 都是从工作的本质出发 而不是像windows那样全都封装好了  这样更能锻炼自身能力
也特别感谢学姐学长的指导和辛勤付出 让我们在学习过程中收益颇丰 
