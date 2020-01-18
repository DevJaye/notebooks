# git的学习笔记

- 初始化文件夹夹
`git init` 
- 查看当前文件的提交状态
`git status` 
- 将库内所有文件提添加进入版本管理
`git add .` 
- 查看变更情况
`git diff` 
- 取消提交
`git reset` 
- 添加用户名和密码
`git config --global user.name "devjaye" ` 
`git config --global user.email "decjaye@163.com" ` 
- //查看自己的用户名和邮箱地址：
git config user.name
git config user.email
- 提交
`git commit -m "提交的描述"` 
`git commit` 什么都不加打开默认文本编辑器
`git commit -a ` 添加并提交,不会添加新建未追踪的文件
修改默认文本编辑器`git config --global core.editor vim` 
- 不想提交某个文件
- 新建文件`.gitignore` 书写忽略文件名
- 已经追踪文件添加至忽略文件无效需要输入
`git rm --cached 文件名称` 告诉git不追踪这个文件,git会告知已经移除此文件
- git 分支
`git branch 名字`
- 切换分支`git checkout 名字`
- 合并分支
`git merge 分支名字` -->合并后分支还在删除分支用`git branch -d 分支名称` <++>

- 提交至github 告知git你的网络上放入git仓库位置
`git remote add origin https://github.com/dj199209/test.git` origin是自己命名的名字
- 查看可推送的分支
`git remote -v` <++>
- 删除提交的分支
git remote remove <name>
- 推送到github
`git push --set-upstream origin master` 
- git记住你的用户名密码
git config credential.helper store`
- git清除缓存密码
`git config --global credential.helper wincred` 
`git credential-manager uninstall` 
- 复制项目
`git clone url` 
- 推送至多个仓库
`git remote set-url --add origin http://mayun.cn/xxx/adsdsdsdcelery-demo.git`
origin为名称
- git remote -v查看提交的仓库
拉取最新的状态拉取到本地
`git pull` 

