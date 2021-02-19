## RPM的使用

### RPM介绍

rpm用于互联网下载包的打包及安装工具，包含在某些Linux发行版中，生成具有.RPM扩展名的文件。RPM是 RedHat Package Manager（RedHat软件包管理工具）的缩写，类似windows的setup.exe

### rpm简单查询命令

查询已安装的rpm列表rpm -qa | grep xxx

### rpm包名基本格式

rpm包名：firefox-60.2.2-1.el7.centos.x86_64

名称：firefox

版本号：60.2.2-1

适用操作系统：el7.centos.x86_64

表示centos7.x的64位系统

如果是i686、i386表示32位系统，noarch表示通用



### rpm命令

#### 查询

rpm -q 软件包名：查询软件包是否安装

rpm -qa：查询所安装的所有rpm软件包

rpm -qi 软件包名：查询软件包信息

rpm -ql 软件包名：查询软件包中的文件

rpm -qf 文件全路径名：查询文件所属的软件包

#### 卸载

rpm -e 软件包名称 

加上--nodeps这个参数可以强制删除

#### 安装

rpm -ivh 软件包全路径名称

-i：安装

-v：提示

-h：进度条



## yum的使用

### 介绍

yum是一个shell前端软件包管理器，基于rpm包管理，能够从指定的服务器自动下载rpm包并且安装，可以自动处理依赖性关系，并且一次安装所有依赖的软件包

### 查询yum服务器是否有需要安装的软件包

yum list | grep xxx软件列表



### yum命令

yum info 软件包名称：查看软件包信息

yum install 软件包名称：安装软件包

yum reinstall 软件包名称：重新安装软件包

yum update 软件包名称：升级软件包

yum remove 软件包名称：卸载软件包

yum clean all：清除所有软件包缓存



