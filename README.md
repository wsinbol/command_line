# command_line

该项目记录各个软件的常用命令行操作及相关配置文件的默认位置，主要针对 Linux 服务器环境。

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



## Git

- git config --global user.email ""
- git config --blobal user.name ""
- git add .
- git commit -m ''
- git remote add <remote_url>
- git push origin master
- git pull origin master
- git checkout -b <branch_name>
- git branch <branch_name>
- git rm -r --cached <file_name> # 删除本地缓存
- git rm -r -n --cached <文件/文件夹名称>  # 加上 -n 这个参数，执行命令时，是不会删除任何文件，而是展示此命令要删除的文件列表预览

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

## Firewall

## 进程&端口
