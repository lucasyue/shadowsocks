Centos7
yum install python-setuptools && easy_install pip
pip install shadowsocks
使用
ssserver -p 443 -k password -m rc4-md5
如果要后台运行：

sudo ssserver -p 443 -k password -m rc4-md5 --user nobody -d start
如果要停止：

sudo ssserver -d stop
如果要检查日志：

sudo less /var/log/shadowsocks.log
用 -h 查看所有参数。你也可以使用 配置文件 进行配置。
