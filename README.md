# protues-use
使用protues实现电路仿真
刚刚开始使用github，上传一个文件夹练习（其中包含使用protues仿真软件对数字电路一些常用电路的仿真）

git上传文件夹练习（本次直接在master主分支开发）
因为git是分布式管理，所以尽量不要在master主分支上作开发

# 操作笔记

# 一.git操作流程：

工作区（加入文件 git add 文件名）-->暂存区（git commit -m ''提交描述）-->本地仓库（git push）-->远程仓库

git status查看当前状态

git clone 仓库地址

初次使用git push 需要输入用户名和密码（添加私有项目权限 git/config文件夹下修改）

# 二.初始化一个新的Git仓库

1.创建一个文件夹

2.初始化git：git init（生成一个隐藏文件）

3.向本地仓库添加文件：
例：touch a1.php

4.修改文件：
vi a1.php
i--插入内容
:wq--保存修改退出vi

5.删除文件：
git rm a1.php

# 分支开发
每次提交本地代码时候，先合并远程master主分支到本地，再提交

1.创建本地分支
git branch 分支名

2.切换本地分支
git checkout 分支名
 
本地分支提交
git  add .
git  commit -m ‘dev'
git push -u origin dev
 
合并本地分支到master

git  checkout master
git pull origin master
git merge origin/master  //合并分支
