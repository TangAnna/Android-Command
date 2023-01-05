##新建分支develop并推送到远程

1.git branch $\color{#FF7D00}{查看本地分支状态}$  
2.git branch -a $\color{#FF7D00}{查看远程分支状态}$  
3.git checkout -b develop $\color{#FF7D00}{创建本地分支develop}$  
4.git branch $\color{#FF7D00}{查看本地分支状态 develop分支 是否创建成功}$  
5.git push origin develop:develop $\color{#FF7D00}{将分支develop推送到远程 远程的名字可以改变也可以同本地分支同名}$  
6.git branch -a $\color{#FF7D00}{查看远程分支 可以查看分支是否成功推送到远程}$  
7.git branch --set-upstream-to=origin/develop develop $\color{#FF7D00}{将本地分支和远程分支进行关联不然pull代码的时候会报错}$  
8.git push origin --delete develop $\color{#FF7D00}{删除远程分支}$  
9.git branch -d delete $\color{#FF7D00}{删除本地分支}$  

##新建tag并推送到远程  
1.git tag $\color{#FF7D00}{查看现有tag状态}$  
2.git tag v1.0 $\color{#FF7D00}{创建tagv1.0}$  轻量标签  
或者 git tag -a v1.0 -m "version1.0版本" $\color{#FF7D00}{创建tag 并添加tag说明}$  附注标签  
3.git tag $\color{#FF7D00}{查看现有tag状态}$  
或者 git show v1.0 $\color{#FF7D00}{查看指定tag的详细信息}$  
4.git push origin v1.0 $\color{#FF7D00}{推送tag v1.0到远程终端}$  
或者git push origin --tags $\color{#FF7D00}{推送所有tag到远程终端}$  
5. git checkout v1.0 $\color{#FF7D00}{切换标签}$  
6.git tag -d v1.0 $\color{#FF7D00}{删除本地tag}$    
7.git push origin —delete tag v1.0 $\color{#FF7D00}{删除远程tag}$  

##合并develop 分支到master  
1.git branch $\color{#FF7D00}{查看分支状态}$  
2.git checkout master $\color{#FF7D00}{切换分支到master上}$  
3.git pull origin master $\color{#FF7D00}{拉取远程master主干代码}$  
4.git merge develop $\color{#FF7D00}{合并develop分支到master上}$  
5.git status $\color{#FF7D00}{查看状态}$  
6.git push origin master $\color{#FF7D00}{如果没有冲突推送到远程master上}$  
7.git checkout develop $\color{#FF7D00}{切换到develop分支，避免下次直接在master上开发}$  

##远程仓库并更时替换Git地址  
git remote set-url origin 新的远程仓库地址  

##查看当前项目的仓库信息  
git remote show origin  
##更新远程分支的代码到当前分支  
git pull origin 任意分支名称  
