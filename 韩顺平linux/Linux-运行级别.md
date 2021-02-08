## 指定运行级别

### 基本介绍

0：关机

1：单用户【找回丢失密码】

2：多用户状态没有网络服务

3：多用户状态有网络服务

4：系统未使用保留给用户

5：图形界面

6：系统重启

常用运行级别是3和5



init（切换不同的运行级别）

获取默认的运行级别：systemctl get-default

设置默认的运行级别：systemctl set-default 设置的级别

​	multi-user.target			运行级别3

​	graphical.target			运行级别5

例如：systemctl set-default multi-user.target 		//设置默认运行级别3



