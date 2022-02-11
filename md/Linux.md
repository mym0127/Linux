Linux

git init : 初始化本地库

​	只有初始化本地库之后目录下的文件才会被Git所管理

git status ：查看本地库状态 

​	有未被追踪的文件时文件名是红色，有存在暂存区但是没有提交到本地的文件时文件是绿色

git diff :查看修改的详细内容

git add 文件名 : 将指定文件添加到暂存区

​	git add 多个文件和文件夹的方法：

 	1.  git add 添加多个文件，文件之间用空格隔开：git add file1 file2 file3
 	2.  git add 文件名，每次添加一个文件添加多次
 	3.  添加指定目录下的文件：git config/*  config目录下及子目录下所有文件,git home/*.php  home目录下的所有.php文件
 	4.  git add . 或者git add --all 添加所有的文件
 	5.  git add 文件夹名

git rm --cached 文件名 ：删除缓存区中的指定文件

 git commit -m"版本信息" 文件名 ：将暂存区中的文件提交到本地版本库

git commit 文件名1 文件名2 -m "版本信息" 中间用空格隔开，可以一次提交多个暂存区中的文件到本地库

git commit -a -m "版本信息"  -a 参数就是可以把还没有执行add命令的修改一起提交

git commit -m"版本信息" 后面不指定文件名，就会将暂存区中的所有未提交文件提交到本地库

git reflog :查看参考日志

git log ：查看详细日志，可以查看到详细的提交人，提交日期

查看日志信息如何退出，在英文输入法下输入q

git reset --hard 7位版本号：实现版本穿越



## 分支

git branch -v: 查看分支

git branch 分支名：创建新的分支

git checkout 分支名：切换分支

git merge 分支名：把指定的分支合并到当前分支上

合并时有冲突如何处理：

​	打开文件手动解决冲突

​	解决完冲突之后，将文件保存并通过git add 命令将文件添加到暂存区

​	通过 git commit - m (后面不要加文件名，不然会报错)的形式将文件提交到本地版本库

​	执行git merge 分支名的命令进行合并

​	注意的是：合并之后被合并的分支的文件是没有变动的，只有合并的分支是解决过冲突的新文件



