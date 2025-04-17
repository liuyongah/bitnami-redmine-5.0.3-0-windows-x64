# bitnami-redmine-5.0.3-0-windows-x64
bitnami-redmine-5.0.3-0-windows-x64-installer

https://softpedia-secure-download.com/dl/b85b7bf298f4c00046e0ac420fdfe47e/67fca8b1/100115249/software/programming/bitnami-redmine-5.0.3-0-windows-x64-installer.exe

简单一键安装还是使用Docker更方便。


下面是 使用 ISO 镜像安装 TurnKey Redmine 的完整步骤教程（适用于 VirtualBox，也适用于实体机/其他虚拟化平台）：

🛠 准备工作
✅ 下载 ISO 镜像
官网地址：
https://www.turnkeylinux.org/redmine
页面中选择 .iso 版本下载。
https://www.turnkeylinux.org/redmine?page=1

✅ 安装 VirtualBox（或 VMware）

✅ 创建新的虚拟机：

名称：Redmine

类型：Linux

版本：Debian (64-bit)

内存建议：1024MB 或以上

硬盘建议：20GB 动态分配

网络模式：桥接（Bridge），确保局域网可访问

🚀 安装步骤（全中文指导）
启动虚拟机，加载 ISO 镜像

在 VirtualBox 中启动新建虚拟机，选择 ISO 镜像作为启动盘。

选择安装类型

第一个选项：Install to hard disk（安装到硬盘）

磁盘分区

一般选择默认即可（使用整个磁盘，自动分区）

设置密码

依次提示你设置：

root 密码（用于 SSH、Web 控制台）

MySQL 密码

Redmine admin 密码（用于登录 Redmine）

配置网络

默认 DHCP，如果你使用桥接模式，一般自动获取 IP

也可以选手动设置静态 IP（建议部署后设置）

系统安装完成，重启

首次启动后，会显示访问信息：

kotlin
复制
编辑
Webmin: https://192.168.1.100:12321
Redmine: http://192.168.1.100/
SSH:    root@192.168.1.100

