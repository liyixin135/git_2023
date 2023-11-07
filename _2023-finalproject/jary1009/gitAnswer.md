# Git Answer
## answer 1
1. way1
> git restore --source==HEAD --stage --worktree file1 file2 ...
> ![picture1](q1way1.png)
1. way2
> git reset HEAD .  
> git checkout -- .
> ![picture2](q1way2.png)


## answer 2
1. way1
> git reset --hard HEAD^  
> ![picture3](q2way1.png)  

2. way2
> git revert HEAD
> ![picture4](q2way3.png) 


## answer 3
1. way1
> git revert HEAD
> ![picture5](q3way1.png)

1. way2
> git rebase master change1   
> 或git checkout change1    
> git rebase master
> ![picture6](q3way2.png)

