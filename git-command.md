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
