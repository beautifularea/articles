备忘  

1 拉取remote指定分支  
git checkout -b iamremotebranch origin/iamremotebranch  

2 删除本地指定分支  
先切换到其他分支，git branch -D iamthebranchneedtobedelete  

3 切换分支  
git checkout iamthebranchneedtobecheck  

4 clone 指定分支  
git clone -b iamthebranch giturl  

5 还原修改过，但未提交的  
git checkout iamthefileneedtorevert

6 查看远程所有分支  
git branch -a  

7 删除remote文件  
git rm file.txt  
git add .  
git commit   
git push  

8 git 重命名文件名  
git mv a.txt b.txt(a->b)  

9 新建分支并切换到新分支  
git checkout -b dev  

10 更新remote列表  
git remote update origin --prune  

11 提交本地resp到remote  
git push origin iamthelocalresp   

12 reset 到某个commit  
git reset --hard commitID  
(commitID后的代码就没有了，慎用！！！）  

13 git fsck --lost-found  
（如果执行12后，后悔了，试试这个操作，去.git/lost_found/other里面找找看有没有）  

14 git revert commit_hash(比如在这个commit_hash上提交的代码要revert)  
1.添加代码xxx, commit后,commit_hash位xxHash.  
2.发现不需要这个代码  
3.git revert xxHash, 并产生一个commit  


--Difference--  
git-revert - Revert some existing commits  
git-reset - Reset current HEAD to the specified state  

git revert is used to record some new commits to reverse the effect of some earlier commits (often only a faulty one).   
If you want to throw away all uncommitted changes in your working directory, you should see git-reset(1).  



