Git is a distributed version control system.
Git is a free software distributed under the GPL.
Git has a mutable index called stage.
Git tracks changes of files.
hello github
Creating a new branch is quick and simple.
--no--ff git merge

git 常用命令
创建版本库：
			创建目录 ———— mkdir name
			进入目录 ———— cd name
			显示文件位置 ———— pwd
			初始化 ———— git init
添加文件：
			添加 ———— git add 文件名
			提交 ———— git commit -m "说明"
查看仓库状态：git status
			查看变化 ———— git diff
版本回退：
			查看历史 ———— git log (--graph) (--pretty=oneline)
			版本回退 ———— git reset --hard HEAD^/ID前几位/HEAD~100
			查看命令历史 ———— git reflog
撤销修改：
			丢弃工作区的修改 ———— git restore <file>
			丢弃暂存区的修改 ———— git restore -- staged <file>
删除文件：
			删除本地文件 ———— rm <file>
			删除仓库文件 ———— git rm <file>		AND		git commit -m "说明"
远程仓库：
			创建SSH ———— ssh -keygen -t -rsa -C "email@email.com"
			关联远程库 ———— git remote add origin git@server-name:path/repo-name.git
			推送 ———— git push (-u) origin <branch-name>
			克隆到本地 ———— git clone 仓库地址
分支管理：
			查看分支 ———— git branch
			创建分支 ———— git branch <name>
			切换分支 ———— git switch <name>
			创建&切换分支 ———— git switch -c <name>
			删除分支 ———— git branch -d <name>
			合并分支 ———— git merge <name>						Fast forward模式
						  git merge --no-ff -m "说明" <name>	--no-ff方式
			储存工作区开辟新工作区 ———— git stash
			恢复并删除新工作区 ———— git stash pop
			查看stash空间 ———— git stash list
			修复复制到其他分支 ———— git cheery-pick
<<<<<<< HEAD
			

=======
			强行删除 ———— git branch -D <name>
>>>>>>> dev
