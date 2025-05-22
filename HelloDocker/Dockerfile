#配置运行环境，node是基于nodeJs的镜像，14是版本号，这个镜像是基于Alpine这个Linux发行版来创建的
FROM node:20-alpine 
# COPY命令是复制文件用的，source指的是相对于Docker的路径，dest是相对于镜像的路径
# COPY source dest
COPY index.js /index.js
# 使用CMD运行应用程序，第一个参数是可执行程序的名字，第二个参数是这个可执行程序接受到的参数
CMD node /index.js

