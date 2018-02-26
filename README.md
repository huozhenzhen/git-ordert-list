# git-ordert-list

整理了一下Git 常用命令，这个版本还是比较好用的，最后附上个人终结版，帮助你快速上手。

取得Git仓库

初始化一个版本仓库

git init
Clone远程版本库

git clone yourgitaddress(你的git地址)
添加远程版本库origin

git remote add origin yourgitaddress(你的git地址)
查看远程仓库

git remote -v
提交你的修改

添加当前修改的文件到暂存区

git add .
如果你自动追踪文件，包括你已经手动删除的，状态为Deleted的文件

git add -u
提交你的修改

git commit –m "你的注释"
推送你的更新到远程服务器,语法为 git push [远程名] [本地分支]:[远程分支]

git push origin master
查看文件状态

git status
跟踪新文件

git add readme.txt
从当前跟踪列表移除文件，并完全删除

git rm readme.txt
仅在暂存区删除，保留文件在当前目录，不再跟踪

git rm –cached readme.txt
重命名文件

git mv reademe.txt readme
查看提交的历史记录

git log
修改最后一次提交注释的，利用–amend参数

git checkout –- readme.txt
基本的分支管理

创建一个分支

git branch workspace
切换工作目录到workspace

git chekcout workspace
将上面的命令合在一起，创建workspace分支并切换到workspace

git chekcout –b workspace
合并workspace分支，当前工作目录为master

git merge workspace
合并完成后，没有出现冲突，删除workspace分支

git branch –d workspace
拉去远程仓库的数据，语法为 git fetch [remote-name]

git fetch
fetch 会拉去最新的远程仓库数据，但不会自动到当前目录下，要自动合并

git pull
查看远程仓库的信息

git remote show origin

个人总结：（其实就小面几行就能满足你一般的上传下载需求）
安装git： npm install git
从git中clone文件，如：git clone https://github.com/...
上传文件：
git add .
git commit –m "你的注释" //要有注释
git push origin master //要指定分支
查看文件状态
git status

 @huozhenzhen
  
            
 
Write  Preview

Leave a comment
选择文件 Attach files by dragging & dropping, selecting them, or pasting from the clipboard.  Styling with Markdown is supported
Comment Close issue
© 2018 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
API
Training
Shop
Blog
About
