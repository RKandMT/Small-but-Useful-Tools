# 本地没有仓库，需要从远程clone
1. 从github中找到远程仓库的clone HTTPS；
2. 在本地仓库目录文件中右键选择Git Bash，打开命令窗口；
3. 输入下面命令，网址字符替换为刚刚复制的远程仓库网址；
```
git clone http://远程仓库网址.git 
```
等待片刻，本地就会有内容啦；
# 从本地更新仓库
1. 先更新本地代码
```
git pull origin main
```

2. 把更新的代码复制进本地仓库文件夹中；

此时如果查看仓库状态：
```
git status
```
则会显示“Untracked file”，即未被追踪到的文件，意思是在文件夹中但不在库中的文件；


3. 代码入库：
```
git add .
```
注意空格句点；

4. 代码提交：
```
git commit -m "描述"
```
此时如果查看仓库状态：
```
git status
```
则会显示“nothing to commit, working tree clean"，即没有待提交的文件；
    
5. 推送至github；
```
git push origin main
```



