# 第一题

## (1):git reset --hard


![1](./Q1-1.png)


## (2):git restore --staged .


![2](./Q1-2.png)




# 第二题

## (1)不修改历史


### git revert -n 版本号


![2-1-1](./Q2-1-1.png)


### git reset --hard


![2-1-2](./Q2-1-2.png)



## (2)修改历史


### git reset --soft HEAD~1


![2-2-1](./Q2-2-1.png)


### git checkout HEAD~1


![2-2-2](./Q2-2-2.png)



# 第三题

## (1)


git checkout master
git cherry-pick [提交编号]


![3-1](./Q3-1)


## (2)
1.  git push --set-upstream origin [分支名】
2.  在github上找到这个分支，开启pull request，然后合并分支


![3-1](./Q3-2-2.1)


![3-1](./Q3-2-2.2)


![3-1](./Q3-2-2.3)


![3-1](./Q3-2-2.4)


