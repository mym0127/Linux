Linux

git init : 初始化本地库

​	只有初始化本地库之后目录下的文件才会被Git所管理

git status ：查看本地库状态 

​	有未被追踪的文件时文件名是红色，有存在暂存区但是没有提交到本地的文件时文件是绿色

git add 文件名 : 将指定文件添加到暂存区

​	git add 多个文件和文件夹的方法：

 	1.  git add 添加多个文件，文件之间用空格隔开：git add file1 file2 file3
 	2.  git add 文件名，每次添加一个文件添加多次
 	3.  添加指定目录下的文件：git config/*  config目录下及子目录下所有文件,git home/*.php  home目录下的所有.php文件
 	4.  git add . 或者git add --all 添加所有的文件
 	5.  git add 文件夹名

git rm --cached 文件名 ：删除缓存区中的指定文件

 git commit -m"版本信息" 文件名 ：将暂存区中的文件提交到本地版本库

git reflog :查看参考日志

git log ：查看详细日志，可以查看到详细的提交人，提交日期

git reset --hard 7位版本号：实现版本穿越
