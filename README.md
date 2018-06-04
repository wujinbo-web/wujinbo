# wujinbo
个人项目仓库
## git 命令行下载 git bash here(git for window)
下载之后一路next 安装
## git指令
1. 基本指令
- git clone git地址
- git config --global user.name "wujinbo-web"
- git config --global user.email "wujinbo@vip.163.com"
- git config --list
- git status  
2. 添加缓存区提交版本区
- git add 文件名
- git add .     (代表添加全部更改的文件到暂存区)
- git commit -m "注释"
- git commit -a -m "注释" (-a代表先添加到暂存区，在添加到版本区)
3. 查看各种提交状态
- git log     (查看提交的版本)
- git diff    (工作区-暂存区)
- git diff --cached/staged (暂存区-版本库)
- git diff master  (工作区-版本库)
4. 撤销
- git reset HEAD 文件名  (从缓存区撤销回来)
- git checkout -- ceshi.html
- git commit --amend  (撤销上一次提交操作)
5. 删除
- git rm 文件名 (删除暂存区文件,工作区必须要删除)
- git rm -f 文件名 (删除工作区和暂存区的文件)
- git rm --cached 文件名 (删除暂存区，工作区不动)
6. 恢复
- git checkout 版本ID 文件名 (恢复某个文件)
- git reset --hard 版本ID    (恢复某个版本)
- git reset --hard HEAD^     (往回一个版本)
- git reset --hard HEAD~2    (回跳多个文件)
- git reflog (查找版本ID，git reset --hard 版本号)
7. 同步到远程仓库
- git 账号是否登录
- git remote (获取远程仓库名字)
- git remote -v (仓库地址)
- git push origin master
8. 多人协助冲突
- git fetch  (git diff master origin/master) (git merge origin/master)
- git pull
9. 分支
- git branch (-d -D  --merged  --no-merged)
- git checkout (-b)
- git merge
10. 标签
### git 三个区
1. 工作区
2. 暂存区
- 作为过渡层，避免误操作
- 不提交不会到版本库，保护工作区和版本区
- 可以进行分支处理
3. 版本区(库)
