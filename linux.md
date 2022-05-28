## CPU&内存

- ps aux --sort -rss 查看内存占用情况

## 磁盘

- df -h 查看整体磁盘使用情况
- du -sh * 查看当前目录每个文件夹的大小
- du -ah --max-depth=1 [/] 查看指定目录各个文件夹占用情况，默认查询当前目录
- du -bsh [/bin/] 查看根目录下bin目录占用情况
- find . size +500M 查找当前目录大于500M的文件

## Firewall

## 进程&端口

- netstat -anp 查看linux系统所有端口占用情况

## FAQ

1. 使用yum报错：Error: rpmdb open failed

```
rm -f /var/lib/rpm/__db*
rpm --rebuilddb
yum -y update
```

2. docker 导致 根目录爆满

> 一般是  /var/lib/docker/overlay2 过大，其一般用来存储 docker 的存储驱动。

```
docker system df // 查看docker容器占用
docker system prune // 清理无用镜像

```

参考博文：https://blog.csdn.net/weixin_32820767/article/details/81196250
