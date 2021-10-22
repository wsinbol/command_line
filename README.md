# command_line

该项目记录各个软件的常用命令行操作及相关配置文件的默认位置，主要针对 Linux 服务器环境。


## Git

- git config --global user.email ""
- git config --blobal user.name ""
- git add .
- git commit -m ''
- git remote add <branch_name> <remote_url>
- git push origin master
- git push origin [local-branch]:[remote-branch] local-branch和remote-branch一般同名 （推送本地分支到远程仓库）
- git pull origin master
- git branch -r 查看远程的所有分支
- git branch -a 查看本地的所有分支
- git branch -vv 查看本地分支与远程分支的映射关系
- git checkout -b <branch_name> 新建分支并切换到该分支
- git checkout <branch_name> 切换到branch_name分支
- git checkout -- <file_name> 撤销对某个文件的修改 （当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时）
- git reset HEAD <file> 从暂存区撤销（已经执行 git add 操作后）当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改
- git switch -c <branch-name> 同上
- git branch <branch_name> 切换到某分支
- git rm -r --cached <file_name>  删除本地缓存，取消对某文件的跟踪。执行此操作后执行git commit 才可以
- git rm -r -n --cached <文件/文件夹名称>  # 加上 -n 这个参数，执行命令时，是不会删除任何文件，而是展示此命令要删除的文件列表预览
- git log -p [application/database.php] 显示某文件每次提交的diff
- git branch -a 查看本地/远程分支
- git push origin --delete [branch_name] 删除远程分支
- git branch -d [branch_name] 删除本地分支
- git branch -r -d [branch_name] 删除远程分支
- git merge --no-ff [branch_name] 将branch_name分支合并到当前分支上
- git cherry-pick [commit-id] 挑选某个分支的单次提交并作为一个新的提交引入到你当前分支上
- git revert 撤回提交信息
- git diff --check (git merge后检查是否还存在有带有冲突标记的文件)
- git rebase -i HEAD~4 (合并多次提交纪录,注意不要合并先前提交的东西，也就是已经提交远程分支的纪录)
- git stash 保存工作现场
- git stash list 查看保存的现场
- git stash pop 恢复工作现场并删除保存记录
- git stash apply stash@{0} 恢复指定的现场
- git log --graph --oneline --abbrev-commit 

- 忽略本地修改，强制用Git仓库的代码覆盖本地代码：

```
git fetch --all
git reset --hard origin/master
git pull
```

- 比较两次commit之间的差异文件

```
git diff hash1 hash2 --stat  
git diff hash1 hash2 <具体的文件>
git diff hash1 hash2 <具体的文件> > patch.txt （将两次提交的差异部分提取成补丁文件）
```

- 奇技淫巧

```
https://github.com/tiimgreen/github-cheat-sheet/blob/master/README.zh-cn.md#%E5%BF%AB%E9%80%9F%E5%BC%95%E7%94%A8
```

- 精彩文章：

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

## Gitlab

- [安装参考博文](https://blog.csdn.net/unhejing/article/details/104767623)

- gitlab-ctl reconfigure: 重载 gitlab 配置
- gitlab-ctl start: 开启 gitlab
- gitlab-ctl stop: 停用 gitlab
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

## CPU&内存

- ps aux --sort -rss 查看内存占用情况

## Firewall

## 进程&端口

## FAQ

1. 使用yum报错：Error: rpmdb open failed

```
rm -f /var/lib/rpm/__db*
rpm --rebuilddb
yum -y update
```
