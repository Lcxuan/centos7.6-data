## 网络配置

修改配置文件指定IP

/etc/sysconfig/network-scripts/ifcfg-网卡名字

```
TYPE=Ethernet				网络类型（通常是Ethemet）
PROXY_METHOD=none
BROWSER_ONLY=no
BOOTPROTO=none				IP的配置方法【none|static|bootp|dhcp】
IPADDR=192.168.34.130
PREFIX=24
DEFROUTE=yes
IPV4_FAILURE_FATAL=no
IPV6INIT=yes
IPV6_AUTOCONF=yes
IPV6_DEFROUTE=yes
IPV6_FAILURE_FATAL=no
IPV6_ADDR_GEN_MODE=stable-privacy
NAME=lcxuan								接口名（设备，网卡）
UUID=43ef170e-66fa-45ca-99c0-d8747401a524	随机ID
ONBOOT=yes								系统启动的时候网络接口是否有效
GATEWAY=192.168.34.2					网关
DNS1=192.168.34.2						域名解析器
```

重启网络服务：service network restart 

查看主机名：hostname

host文件：/etc/hostname