---
title: Shell专题解读
date: 2023-12-17 23:23:36
tags: Shell, Nginx,Server开发
---

# Shell Topics

> 服务端运维-管理：开发，主题方式深入内核，中间件，体系结构-CPU

## 服务器开发

> 常见场景解析
>
> - 服务之间网络通信路径，Ping通，TCP访问不到：涉及路由表-ECMP,防火墙，TCP/IP协议选择路径-hash五元组
> - Nginx配置

### 观测与判断

> 脚本语法部分：不够专 -> 拿OS脚本 **训练**

- 服务状态

  > 可检测的范围： nginx手动启动，service, systemctl无法观测到？

  - service :  运行/etc/init.d/xxx.sh
    - service --status-all: ufw[+] -> {runninng}, 但是ufw status : inactive -> **怎么解释**
  - systemctl ： systemd, {/etc/systemd/***}
  - ps

- 磁盘设备挂载信息： du -h | sort -hr

- 

### 安装与源码

> 安装与配置，生效优先级
>
> - PMS的默认行为：
> - 源码安装：
>
> 冲突问题： make install -> /usr/bin/xxx, 配置文件 -> /etc/xxx/conf

- PMS工具设计与实现： rpm , dpkg -> aptitude:前端展示
  - 对应软件安装信息使用的数据库如何设计与实现？ - 软件包，安装文件信息
  - 对远端repository，访问工具
  - 软件包依赖关系检测
- 
- 





## 存储管理

### FS文件系统







## 进程管理



### 虚拟进程

> 软件框架 - 套壳工具
>
> - 常见：**微信分身工具**，
> - App开发，桌面客户端开发





