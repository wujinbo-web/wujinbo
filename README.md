# wujinbo
个人项目仓库
## git 命令行下载 git bash here(git for window)
下载之后一路next 安装
## git指令
- git clone git地址
- git config --global user.name "wujinbo-web"
- git config --global user.email "wujinbo@vip.163.com"
- git config --list
- git status  
- git add 文件名
- git add .     (代表添加全部更改的文件到暂存区)
- git commit -m "注释"
- git commit -a -m "注释" (-a代表先添加到暂存区，在添加到版本区)
- git log     (查看提交的版本)
- git diff    (工作区-暂存区)
- git diff --cached/staged (暂存区-版本库)
- git diff master  (工作区-版本库)
- git reset HEAD 文件名  (从缓存区撤销回来)
- git checkout -- ceshi.html
### git 三个区
1. 工作区
2. 暂存区
- 作为过渡层，避免误操作
- 不提交不会到版本库，保护工作区和版本区
- 可以进行分支处理
3. 版本区(库)
