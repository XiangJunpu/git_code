# git_code

1.mkdir learngit %创建一个名称为learngit文件夹

2.cd learngit %切换工作目录至learngit

3.pwd %（print working directory）输出当前工作目录的绝对路径

4.git init %命令执行完后会在当前目录生成一个.git目录

5.git add readme.txt %把文件read.txt添加暂存区

6.git commit -m "wrote a readme file" %把暂存区的所有内容提交到当前分支，引号里的是本次提交的说明

7.git status %用来查看仓库的状态

8.git diff readme.txt %用于比较readme.txt修改前后的不同

9.git log %命令显示从最近到最远的提交日志

10.git reset --hard HEAD^ %将当前版本回退到上一个版本，HEAD表示当前版本，上一个版本就是HEAD^，上上一个版本就是HEAD^^，往前100个版本可以写成HEAD~100

11.git reflog %查看命令历史，以便确定要回到未来的哪个版本

12.cd .. %返回上一个目录

13.git checkout -- readme.txt %把readme.txt文件在工作区的修改全部撤销，这里有两种情况：（1）是readme.txt自修改后还没有被放到暂存区，
现在，撤销修改就回到和版本库一模一样的状态（2）是readme.txt已经添加到暂存区后，又做了修改，现在，撤销修改就回到添加到暂存区后的状态。
总之,就是让这个文件回到最近一次git commit或git add时的状态。

14.git reset HEAD readme.txt %如果文件已经通过 git add 添加到暂存区，在 git commit 前又想进行撤回，用命令 git reset HEAD <file> 可以把暂存区的修改撤销掉，重新放回工作区，然后再用git checkout --readme.txt进行撤销
  
15.删除文件：如果确定要删除，则（1）rm test.txt （2）git commit -m "remove test.txt"
            如果是错删了，则（1）rm test.txt （2）git checkout -- test.txt 因为版本库里还有，所以可以很轻松的把误删的文件恢复到最新版本。（用版本库里的版本替换工作区的版本）
     
16.git remote add origin git@github.com:XiangJunpu/learngit.git %将已有的本地仓库与github上的仓库进行关联
   git push -u origin master %把本地库的所有内容推送到远程库上，把当前分支master推送到远程，由于远程库是空的，第一次推送就加上 -u 参数。
   git push origin master %把本地master分支的最新修改推送到GitHub。

17.git clone git@github.com:XiangJunpu/gitskills.git %从远程库克隆仓库gitskill到本地库

18.git checkout -b dev %表示创建了分支，并切换到dev分支 （等价于git branch dev, git checkout dev）

19.git branch %会列出所有分支，当前分支前面会标一个 * 号

20.git checkout master %将分支切换回master分支

21.git merge dev %用于合并指定分支到当前分支

22.git branch -d dev %删除分支dev  （因为创建、合并和删除分支非常快，所以Git鼓励你使用分支完成某个任务，合并后再删除分支，这和直接在master分支上工作效果是一样的，但过程更安全）

23.vi readme.txt %进入文本编辑  esc, :wq 保存并退出编辑

24.





