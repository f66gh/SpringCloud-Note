## 基本概念

Docker是一个用于构建、运行、传送应用程序的平台。

有了docker，可以将OS、运行环境、第三方软件库和依赖包、配置文件与启动命令等一起打包传送给另一台主机。

## Docker与虚拟机的区别

### 虚拟机问题

我们可以在一台主机上配置多个逻辑主机，在实际开发中每一个逻辑主机只需要对外提供某一种特定的服务。如果用我们在一台主机上构建多个虚拟机，由于每一个虚拟机都会占有CPU，RAM，硬盘等，所以对于上述要求成本高，此外由于每台虚拟机需要独立运行一个OS，启动速度慢，又进一步加大了运行成本。

### 容器

容器是容器，Docker是Docker。

Docker是容器的一个实现，是容器化的一个解决平台。

容器和虚拟机类似，是一个独立的环境。与虚拟机的区别是不需要使用额外的OS，直接使用宿主的OS。

![image-20250506165157738](C:\Users\BaiMu\AppData\Roaming\Typora\typora-user-images\image-20250506165157738.png)

## 基本原理

类比于Java，镜像是模板（类），容器是模板的一个实例（对象），可以有一个也可以有多个。

仓库是存储镜像的地方，主要用途是镜像的共享和复用。

![image-20250506165459570](C:\Users\BaiMu\AppData\Roaming\Typora\typora-user-images\image-20250506165459570.png)

## 容器化和Dockerfile

Dockerfile是一个文本文件，里面包含指令，用来告知Docker如何构建镜像，并且包含了各种依赖、配置环境和运行程序所需要的所有内容。

![image-20250506220419895](C:\Users\BaiMu\Desktop\SpringCloud-Note\docker\pic\image-20250506220419895.png)

## Docker Compose

Docker Compose用于定义和运行多容器Docker应用程序的工具。

Docker Compose可以将各个不同的业务关联组合在一起（如Vue+SpringBoot+MySQL），当需要配置环境时直接一行代码解决。
