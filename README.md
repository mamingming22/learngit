# learngit
学习git的项目
学习git的命令 掌握如何操作项目的pull push clone等等


git local 测试
1.新建了gitlocal.md，并放入文件夹
2.git add gitlocal.md 将gitlocal。md放到暂存区
3.git commit -m "message"
试试gui怎么用
4.git log 查看历史纪录
5.git reset --hard commit_id 可以回退到某个版本
git reset --hard HEAD^ 可以回到上个版本

git reset HEAD README.md 把暂存区readme文件的修改撤销
再用git checkout -- README.md 将修改清理掉
若是回错版本
6.git reflog 命令查看命令历史
然后可以选择要回到的那个版本

//新加入了一行，在位提交之前用git checkout -- file.name可以清掉自上次提交后修改的地方

1.git init      -------创建空的版本库；
2.git add       -------添加文件到暂存区；
3.git commit      -------提交文件到版本库(仓库)；
4.git status      -------查看相关状态；
5.git diff      -------查看具体修改的内容；
6.git log      -------查看提交历史记录；
7.git reset      -------回到上一版本；
8.git reflog      -------查看命令历史记录；
9.git checkout      -------丢弃工作区的修改；
10.git rm      -------删除文件；

use vim test

creating a new branch
git checkout -b dev相当于git branch dev & git checkout dev
git merge dev 合并dev分支到master上

Git鼓励大量使用分支：

查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>
------------------------------------------------------------
因此，多人协作的工作模式通常是这样：

首先，可以试图用git push origin branch-name推送自己的修改；

如果推送失败，则因为远程分支比你的本地更新，需要先用git pull试图合并；

如果合并有冲突，则解决冲突，并在本地提交；

没有冲突或者解决掉冲突后，再用git push origin branch-name推送就能成功！

如果git pull提示“no tracking information”，则说明本地分支和远程分支的链接关系没有创建，用命令git branch --set-upstream branch-name origin/branch-name。
