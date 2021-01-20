# command_line

该项目记录各个软件的常用命令行操作及相关配置文件的默认位置，主要针对 Linux 服务器环境。

## Gitlab

- gitlab-ctl reconfigure: 重载 gitlab 配置
- gitlab-ctl start: 开启 gitlab
- gitlab-ctl stop: 停用 gitlab
- gitlab-ctl restart:
- gitlab-ctl status: 查看 gitlab 运行环境状态
- gitlab-ctl tail: 查看 gitlab 实施日志

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
