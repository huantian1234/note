###### docker
### docker run命令
-i 以交互式操作

-t 终端

-d 在后台运行

-P 容器内开发的端口随机映射

-p [主机端口]:[容器端口]

-v [主机目录]:[容器目录]

/bin/bash 交互性shell放在容器名后面

### docker基本操作
docker ps -a 查看所有容器

### docker exec 
docker exec -it [id] /bin/bash

进入容器shell

exit退出

### Dockerfile
docker build -t [容器名]:[版本编号] . <-点指当前目录

作用:构建 . 目录下的 Dockerfile
