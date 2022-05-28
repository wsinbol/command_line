# Docker

- docker ps 查看正在运行的容器
- docker ps -a 查看所有容器信息
- docker ps -a -q 查看所有容器ID
- docker stop $(docker ps -a -q)   停止所有容器
- docker rm $(docker ps -a -q) 删除所有容器
- docker exec -it <container_id/name> /bin/bash   进入容器shell
- docker exec -it <container_id/name> /bin/sh    进入容器shell，当镜像是使用alpine制作时
