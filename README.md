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
