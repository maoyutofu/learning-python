# 第二天学习课题
实现一个类似虚拟主机分配的东西。以Nginx作为web服务器，可以操作Nginx配置文件，分配N个虚拟主机。以分配的域名作为虚拟主机root目录和配置文件。当一个用户从命令行界面输入一个域名，就可以根据域名在Nginx中创建一个新的虚拟主机也就是server节点。

## usage
``` shell
python vhost.py dev-tang.com
```
不直接操作nginx.conf的server节点，而是每个虚拟主机都创建一个新的配置文件，以include的方式到nginx.conf
