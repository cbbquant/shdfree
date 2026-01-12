# 软件简介
CBB超级套利免费版是一款加密货币对冲套利软件，支持各主流交易所的现货vs现货，永续vs永续以及现货vs永续的对冲套利。
## 部署要求
需要独立的拥有公网IP的服务器，可在亚马逊云、阿里云、腾讯云等租用符合要求的服务器<br/>
操作系统：centos 7.x或centos 8.x<br/>
最低硬件：2核2G
## 软件安装
使用PuTTY或其他SSH管理软件连接并登录您的服务器，在命令行中输入如下代码，耐心等待服务器下载安装包并自动安排。
```bash
rpm -ivh https://github.com/cbbquant/shdfree/releases/latest/download/cbbshdfree.rpm
```
注意事项：非root权限请在上述安装命令前加sudo，如下所示：
```bash
sudo rpm -ivh https://github.com/cbbquant/shdfree/releases/latest/download/cbbshdfree.rpm
```
## 验证安装
在服务器命令行中输入如下代码并回车：
```bash
systemctl status cbbshdfree
```

# 开始使用
## 登录软件
在浏览器中输入http://您的服务器公网IP:6680/，如果无法打开相应网址，
