# 笔记
### 查看配置
	$ git config --list
### 获取帮助
	 $ git help
### 创建仓库
	 $ git init
### 克隆
	 $ git clone  URL
### 检查文件状态
	$ git status

新添加的未跟踪文件： `?? `，

新添加到暂存区中的文件：` A `，

修改过的文件： `M `

右边的` M `表示：该文件被修改了但是还没放入暂存区；左边的 `M` 表示：该文件被修改了并放入了暂存区。 

### 创建一个文件
	' $ echo 'My Project' > README
 
一个\>是覆盖输入，两个\>\>是追加
### 提交
	git commit -a -m '说明文字'


-a:跳过暂存，提交所有

	git commit -amend


重新提交


### 查看提交历史

	git log

很多参数可以跟在后面
### 取消暂存的文件

	git reset HEAD <file>

### 取消修改

	git checkout -- <file>

### 添加远程仓库

	git remote add <shortname> <url>

重命名：

	$ git remote rename <shortname1> <shortname2>

移除：

	$ git remote rm <shortname2>


### git fetch 和git pull
fetch 将远程主机的最新内容拉到本地，检查之后再合并（merge）
pull=fetch+merge

### 分支创建
——在当前指针`HEAD`上创建一个新的分支，不会自动切换到新的分支去。
	git branch  <branch-name>


创建并切换到该分支：

	git branch -b <name>

### 分支切换：

	git checkout <name>

切换分支会改变你的工作目录中的文件。——你的工作目录会回复到该分支最后一次提交时的样子。
