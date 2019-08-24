<center><h2 style=color:red><b>Git教程</b></h2></center>
https://blog.csdn.net/gudujianw/article/details/80965067

https://baijiahao.baidu.com/s?id=1594979541273085800&wfr=spider&for=pc

https://blog.csdn.net/weixin_43211277/article/details/82715355  如何解决git上传文件出错[rejected] master -> master (fetch first) error: failed to push some refs to '
https://blog.csdn.net/qq_38716242/article/details/79380825
Git安装

1. 设置用户名和邮箱，作为一个标识。

   ```git
   $ git config --global user.name "Jivan"
   $ git config --global user.email"wen170@gmail.com"
   ```

2. 输入 ssh-keygen ，按三次enter

##### Git基本常用命令如下**

mkdir：        XX (创建一个空目录 XX指目录名)

pwd：          显示当前目录的路径。

git init          把当前的目录变成可以管理的git仓库，生成隐藏.git文件。

git add XX       把xx文件添加到暂存区去。

git commit –m “XX”  提交文件 –m 后面的是注释。

   git status        查看仓库状态

   git diff  XX      查看XX文件修改了那些内容

   git log          查看历史记录

   git reset  –hard HEAD^ 或者 git reset  –hard HEAD~ 回退到上一个版本

​                        (如果想回退到100个版本，使用git reset –hard HEAD~100 )

   cat XX         查看XX文件内容

   git reflog       查看历史记录的版本号id

   git checkout — XX  把XX文件在工作区的修改全部撤销。

   git rm XX          删除XX文件

   git remote add origin https://github.com/wen1710/www.git   关联一个远程库

   git push –u(第一次要用-u 以后不需要) origin master 把当前master分支推送到远程库

   git clone https://github.com/wen1710/www.git  从远程库中克隆

   git checkout –b dev  创建dev分支 并切换到dev分支上

   git branch  查看当前所有的分支

   git checkout master 切换回master分支

   git merge dev    在当前的分支上合并dev分支

   git branch –d dev 删除dev分支

   git branch name  创建分支

   git stash 把当前的工作隐藏起来 等以后恢复现场后继续工作

   git stash list 查看所有被隐藏的文件列表

   git stash apply 恢复被隐藏的文件，但是内容不删除

   git stash drop 删除文件

   git stash pop 恢复文件的同时 也删除文件

   git remote 查看远程库的信息

   git remote –v 查看远程库的详细信息

   git push origin master  Git会把master分支推送到远程库对应的远程分支上





Step 1:

安装git

新建一个文件夹作为git本地仓库

```
git init             
```

把当前的目录变成可以管理的git仓库，生成隐藏.git文件。

step 2：

```git
git clone https://github.com/wen1710/www.git  从远程库中克隆
```

通过命令 git clone [仓库链接]将中央代码仓库下载到本地。下载的仓库会保存到输入命令时所在的位置。

step 3:

推送修改到中央代码仓库共分 3 步。首先，暂存（stage）文件，告诉 Git 希望将哪 个修改过的文件推送到中央代码仓库。

```
git add [文件名]
```

将文件加入缓存

```
git commit -m "备注更新内容"
```

提交文件，即 命令 Git 记录本地代码仓库所做的修改。 可使用语法 git commit -m [信息]提交 文件。 该命令将创建一次提交（commit）：Git 保存的一个项目代码版本。 旗标-m 表示要添加一段信息， 帮助记忆对项目做了什么修改以及原因（这条信息类似注释）。

step 4：

```
git push origin master
```

提交文件后，即可进行最后一步。可通过命令 git push origin master，将本地的修改推送到中央代码库：

step 5:

```
git pull origin master
```

我们可以使用命令 git pull origin master 更新本地代码仓库：Git 会把中央代码仓库的修改应用到本地。









   