---
layout: article
title: Git命令清单
---

`git init`

**新建**版本库。目录下会多一个.git文件夹。

`git add <file>`

将`<file>`文件加入**暂存区**。

`git commit -m "comment"`

将**暂存区**内容提交到**当前分支**。

`git status`

查看当前仓库**状态**。

`git reset --hard HEAD^`

返回上一个版本。

`git reset --hard HEAD^^`

返回上上一个版本。

`git reset --hard HEAD~n`

向上返回n个版本。

`git reset --hard (comment id)`

返回到版本号所在版本（不需要写全版本号，只需要写前几位）

`git reflog`

查看每一次记录的命令（查找版本号用）

`git diff HEAD -- <file>`

查看工作区和版本库里面最新版本的区别。

`git checkout --<file>`

把文件在工作区的修改全部撤销。有两种情况：

①修改后还没有提交到暂存区，撤销修改会回到和版本库一样的状态。

②修改后添加到的暂存区，撤销修改会回到暂存区状态。

`git reset HEAD <file>`

把暂存区修改撤销掉，重新放回工作区。

`git rm <file>`

从版本库删除文件。

`ssh-keygen -t rsa -C "youremail@example.com"`

创建ssh Key。在用户目录里面可以看到`.ssh`目录。有`id_rsa`和`id_rsa.pub`两个文件。后者是公钥，可以告诉任何人。