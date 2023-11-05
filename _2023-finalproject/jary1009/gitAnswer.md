# Git Answer
## answer 1
1. way1
> git restore --source==HEAD --stage --worktree file1 file2 ...
<img src="q1way1.png" width="100%">
2. way2
> git reset HEAD .  
> git checkout -- .
> <img src="q1way2.png" width="100%">  


## answer 2
1. way1
> git reset --hard HEAD^  
> <img src="q2way1.png" width="100%">  

2. way2
> git reset --soft a448e2e(版本号)
> <img src="q2way2.png" width="100%"> 


## answer 3
1. way1
> git merge change1
> <img src="q3way1.png" width="100%">  

1. way2
> git rebase master change1   
> 或git checkout change1    
> git rebase master
> <img src="q3way2.png" width="100%"> 

