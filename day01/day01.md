# 第一天学习课题
实现一个端口扫描器。输入一个服务器ip地址，返回这台服务器所开放的端口，以及端口在被什么程序使用。也可以按指定端口进行范围扫描。

## usage
1. 扫描所由的端口，只显示open：
``` shell
python scaner.py 192.168.1.111
[+]22/tcp open
SSH-2.0-OpenSSH_7.2p2
```

2. 扫描指定范围内的端口，显示open与close
``` shell
python scaner.py 192.168.1.111 22:25
[+]22/tcp open
[-]23/tcp closed
[-]24/tcp closed
[-]25/tcp closed
```
