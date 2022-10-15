# 序

目前包含 git 、gitlab 常用命令行操作。

- [firstaidgit.io](http://firstaidgit.io/) 一个可搜索的最常被问到的Git的问题
- [git-extra-commands](https://github.com/unixorn/git-extra-commands) - 一堆有用的额外的Git脚本

# Git

## 基础操作
- git init [directory] 初始化仓库
- git clone <repo> 克隆远程仓库到本地
- git config --global user.email ""
- git config --global user.name ""
- git add .
- git commit -m ''
- git status 显示哪些文件已被staged、未被staged及未跟踪untracked
- git checkout - 快速切换到上一个分支


##  合并操作

- git merge --no-ff [branch_name] 将branch_name分支合并到当前分支上
- git cherry-pick [commit-id] 挑选某个分支的单次提交并作为一个新的提交引入到你当前分支上
- git diff --check (git merge后检查是否还存在有带有冲突标记的文件)

##  版本操作
- git revert <commit_id> 令当前分支回退到commit_id时的状态
- git checkout -- <file> 撤销对某个文件的修改 （当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时）
- git reset <file> 将file从暂存区移除，但保持工作区不变，此操作不会修改工作区的任何文件
- git reset HEAD <file> 从暂存区撤销（已经执行 git add 操作后）当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改
- git reset --hard HEAD^ 回退到上一个版本 （回退到上两个版本的话用HEAD^^，以此类推）
- git reset --hard <commit-id> 回退到指定版本
- git rm --cached <file> 取消对某文件的跟踪，但保留本地文件
- git rm -r -n --cached <文件/文件夹名称>  # 加上 -n 这个参数，执行命令时，是不会删除任何文件，而是展示此命令要删除的文件列表预览
- git rm -r --cached <file>  删除本地缓存，取消对某文件的跟踪。执行此操作后务必执行git commit，不要执行git add 
- git revert 撤回提交信息
- git rebase -i HEAD~4 (合并多次提交纪录,注意不要合并先前提交的东西，也就是已经提交远程分支的纪录)



## 对比操作

- git diff 不加参数默认比较工作区与暂存区的变化
- git diff HEAD 比较工作区和最近一次commit的变化
- git diff --cached [file_name] (比较暂存区与最新本地版本库【即本地库中最近一次commit的内容】)
- git diff hash1 hash2 --stat  以统计形式对比2次提交的变化
- git diff hash1 hash2 <具体的文件> 查看某个文件在两个提交中的具体变化
- git diff hash1 hash2 <具体的文件> > patch.txt （将两次提交的差异部分提取成补丁文件）


##  远程操作


- git remote add <repo_name> <remote_url> 关联远程仓库
- git push [origin] [master] 推送master的修改到origin仓库
- git push origin [local-branch]:[remote-branch] local-branch和remote-branch一般同名 （推送本地分支到远程仓库）
- git remote -v 查看仓库地址
- git remote rm origin  删除仓库
- git fetch --all 拉取远程仓库所有信息到本地缓存
- git pull origin master 拉取master分支并快速合并




##  分支操作


- git branch 查看本地分支
- git branch -r 查看远程的所有分支
- git branch -a 查看本地/远程的所有分支
- git branch -vv 查看本地分支与远程分支的映射关系
- git checkout -b <branch_name> 新建分支并切换到该分支
- git switch -c <branch-name> 新建分支并切换到该分支
- git branch <branch_name> 新建某分支但不切换
- git checkout <branch_name> 切换到branch_name分支
- git branch -m <master> <main> 重命名本地分支，将master分支移到main（因为github将master分支改为main所致）
- git push origin --delete dev 删除远程dev分支
- git branch -d dev 删除dev本地分支
- git branch --merged master | grep -v '^\*\|  master' | xargs -n 1 git branch -d 删除已经合并到 master 的分支



> 在使用HTTP方式拉取代码时一定要重视这些操作，因为默认拉下来的只有 master 分支，其他分支只能自己创建并关联！
```
1. git branch -r // 查看远程分支
2. git branch -vv // 查看本地分支与远程分支的映射关系
3. git fetch <origin> <远程分支命名>:<本地分支命名> // 将远程分支拉取到本地
4. git checkout <本地分支命名> // 切换到新拉取的本地分支
5. git branch -u <origin/develop> // 建立本地分支与远程分支的映射 或者使用 git branch --set-upstream-to origin/develop
6. git branch -vv // 再次确认本地分支与远程分支映射关系

- git branch --unset-upstream // 撤销本地分支与远程分支的映射关系
```


##  标签操作

- git tag [v1.0] 打标签
- git tag 查看所有标签
- git tag -a <tagname> -m "blablabla..." 添加备注信息并打标签
- git tag -d [v1.0] 删除本地标签
- git push origin [v1.0] 推送指定标签
- git push origin --tags 推送所有标签
- git push origin :refs/tags/[v1.0] 删除远程标签
- git push origin --delete tag <tagname> 删除远程标签
- git checkout -b branch_name tag_name 回退到某个标签

------

##  草稿操作

```
- git stash 保存工作现场
- git stash list 查看保存的现场
- git stash pop 恢复工作现场并删除保存记录
- git stash apply stash@{0} 恢复指定的现场
- git stash show -p stash@{1} 查看某个stash具体内容
```

##  日志操作

- git log -p [application/database.php] 显示某文件每次提交的diff
- git log --graph --oneline --abbrev-commit  可视化查看提交情况

> 如何查看某个文件的修改历史？

```
1. git log --pretty=oneline <file_path+file_name>  先列出指定文件的所有改动历史
2. git show <commit_id> 查看某个提交的详细信息
3. git show <commit_id> <fileName> 查看某个提交中某个文件的变化
```

## 常见情景

- git commit 配置提交模版

```
1. 新建 .gitmessage 文件，具体见同级目录 .gitmessage 文件
2. git config --global commit.template "D:\java-project\zhongyi-cloud\.gitmessage"
3. 输入 git commit 后回车
4. 根据提示写内容
```

- 忽略本地修改，强制用Git仓库的代码覆盖本地代码：

```
git fetch --all
git reset --hard origin/master
git pull
```

- gitlab修改账户密码后提示：Authentication failed

```
打开控制面板 =》用户账户 =》 管理windows 凭据，修改对应凭据的密码即可！
```


- centos7解决git每次都要输入账号密码的问题

```
git config --global user.name "用户名"
git config --global user.email "邮箱"
find / -name .gitconfig
在 .gitconfig 文件中加入：

[credential]
	helper = store

切换到项目目录执行：git config --global credential.helper store
```

- Github使用秘籍

```
https://github.com/tiimgreen/github-cheat-sheet/blob/master/README.zh-cn.md#%E5%BF%AB%E9%80%9F%E5%BC%95%E7%94%A8
```

## 参考资料
- https://github.com/521xueweihan/git-tips#%E5%9B%9E%E5%88%B0%E8%BF%9C%E7%A8%8B%E4%BB%93%E5%BA%93%E7%9A%84%E7%8A%B6%E6%80%81

```
https://www.ruanyifeng.com/blog/2015/08/git-use-process.html
https://willi.am/blog/2014/08/12/the-dark-side-of-the-force-push/
https://www.ruanyifeng.com/blog/2012/07/git.html

rebase:
http://jartto.wang/2018/12/11/git-rebase/
```

- 结合crontab命令自动push到远程仓库

```
#!/bin/bash
source /etc/profile
cd /www/wwwroot/lejin.yunmell.com
ls
git add .
git commit -m 'auto push'
git push origin master
```

> 当手动执行脚本OK，但是 crontab 死活不执行时,很可能是环境变量惹的祸，可尝试在crontab中或者bash脚本中直接引入环境变量解决问题。上面的source一行就是引入环境变量用的。

其他注意事项：
> 1. 脚本中涉及文件路径时写全局路径；
> 2. 脚本执行要用到java或其他环境变量时，通过source命令引入环境变量

- 一键提交脚本

```
#!/bin/bash

if [ -z "$(git status --porcelain)" ];
then
    echo "IT IS CLEAN"
	exit 0
fi

echo "Enter your message"
read message
if [ -z "${message}" ];
then
	message="update"
fi

git add .
git commit -m"${message}"
echo "Pushing data to remote server!!!"
git push -u origin master

exit 0
```

# Gitlab

- [安装参考博文](https://blog.csdn.net/unhejing/article/details/104767623)

- gitlab-ctl reconfigure: 重载 gitlab 配置
- gitlab-ctl start: 开启 gitlab
- gitlab-ctl stop: 停用 gitlab
```
systemctl stop gitlab-runsvdir // 只执行上面的命令并不能彻底结束gitlab相关进程，遗留的进程仍占用CPU和内存
```
- gitlab-ctl restart:
- gitlab-ctl status: 查看 gitlab 运行环境状态
- gitlab-ctl tail: 查看 gitlab 实时日志
- head -1 /opt/gitlab/version-manifest.txt 查看gitlab版本
- gitlab-ctl stop unicorn 关闭gitlab 数据连接
- gitlab-ctl stop sidekiq 关闭 sidekiq
- rpm -e [gitlab-ce] 卸载 gitlab
- find / -name *gitlab*|xargs rm -rf 深度卸载
- find / -name gitlab |xargs rm -rf  深度卸载

配置修改文件：
/etc/gitlab/gitlab.rb

*最新版本的gitlab已经弃用unicorn*

```
修改访问IP：
external_url 'http://60.205.194.237:9002'

指定端口
nginx['listen_port'] = 9002

依据情况决定是否修改
unicorn['port'] = 9191

```

gitlab默认备份文件：
/var/opt/gitlab/backups
