## 1:
-- git reset <参数> \[指定commit\]:
回退至指定commit处,并将其之后的修改...
* 保留在暂存区中 (--soft参数)
* 完全不保存  (--hard参数)
* 保留在工作区 (无参数或 --mixed参数)

-- git reset HEAD filepathname
大约相当于git add 的反指令
## 2:
-- git reset --hard head\[参数\]
* head指当前版本
* head^指上一个版本
* head^^指上上个版本
* head~3指回退三个版本

## 3:
-- git rebase \[main line\] \[other lines\]
* 将\[other lines\]中的数据直接合并到\[main lines\]
* 或者说是将\[other lines\]中的修改与\[main lines\]对比,提取,应用
-- 