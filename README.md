# 软件简介
CBB超级套利免费版是一款加密货币对冲套利软件，支持各主流交易所的现货vs现货，永续vs永续以及现货vs永续的对冲套利。
## 硬件要求
需要拥有独立的公网IP的服务器，可在亚马逊云、阿里云、腾讯云等租用符合特定网络(如可直接访问交易所官网)要求的服务器<br/>
操作系统：centos 7.x或centos 8.x<br/>
最低硬件：2核2G
## 软件安装
使用PuTTY或其他SSH管理软件连接并登录您的服务器，在命令行中输入如下代码，耐心等待服务器下载安装包并自动安装。
```bash
rpm -ivh https://github.com/cbbquant/shdfree/releases/latest/download/cbbshdfree.rpm

或

rpm -ivh http://down.xitour.com/shd/cbbshdfree.rpm

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
如在命令行窗口看到“Active: active (running)”字样，则表示软件已正常运行<br/>
本地电脑浏览器打开管理网址：
```bash
http://您的服务器公网IP:6680/
```

## 检查可访问性
在你本地电脑的浏览器中输入`http://您的服务器公网IP:6680/`，如果无法访问，则检查“云服务器安全组(防火墙)”和“操作系统防火墙”这两项，
#### 1、云服务器安全组(防火墙)
登录云服务器控制台，确保云服务器所在安全组(防火墙)开放了6680端口
#### 2、操作系统防火墙
在云服务器安全组(防火墙)确认已开放了6680端口后，如果仍然无法正常访问，请在操作系统防火墙中开放6680端口，具体方法请查阅搜索引擎解决。

# 开始使用
在您本地电脑的浏览器中输入`http://您的服务器公网IP:6680/`，如果无法打开相应网址，请重新执行“验证安装”和“检查可访问性”这两个条目，软件初始登录时，未配置任何登录账户，登录时的登录选项请选择“通讯密钥”登录，默认密码为123456，登录后请立即修改通讯密钥，最后在软件中的“通用配置”-->“软件授权”里，登录您的邮箱即可开始使用，登录邮箱仅为方便开发者统计数据，不影响软件的免费使用。
# 支持的交易所
|名称|交易所代码|类型|折扣|注册|
| :- | :- | :- | :- | :- |
| 币安现货|ba|现货|20%|[注册账户](https://accounts.binance.com/register?ref=HE58BXUN)|
| 币安USDT永续|bac|永续合约|20%|[注册账户](https://accounts.binance.com/register?ref=HE58BXUN)|
| 币安USDC永续|bab|永续合约|20%|[注册账户](https://accounts.binance.com/register?ref=HE58BXUN)|
| 币安币本位永续|bap|永续合约|20%|[注册账户](https://accounts.binance.com/register?ref=HE58BXUN)|
| 币安币本位交割|bas|交割合约|20%|[注册账户](https://accounts.binance.com/register?ref=HE58BXUN)|
| 欧易现货|ok|现货|20%|[注册账户](https://www.okx.com/join/XCBBLA)|
| 欧易USDT永续|okp|永续合约|20%|[注册账户](https://www.okx.com/join/XCBBLA)|
| 欧易币本位永续|oks|永续合约|20%|[注册账户](https://www.okx.com/join/XCBBLA)|
| 欧易USDT交割|oku|交割合约|20%|[注册账户](https://www.okx.com/join/XCBBLA)|
| 欧易币本位交割|okc|交割合约|20%|[注册账户](https://www.okx.com/join/XCBBLA)|
| Bybit现货|by|现货|33%|[注册账户](https://partner.bybit.com/b/cbbla)|
| BybIT永续USDT|byu|永续合约|33%|[注册账户](https://partner.bybit.com/b/cbbla)|
| BybIT永续USDC|byp|永续合约|33%|[注册账户](https://partner.bybit.com/b/cbbla)|
| 火必现货|hb|现货|---|[注册账户](https://www.htx.com/invite/zh-cn/1f?invite_code=cbbla)|
| 火必USDT永续|hbp|永续合约|---|[注册账户](https://www.htx.com/invite/zh-cn/1f?invite_code=cbbla)|
| Gate现货|gt|现货|20%|[注册账户](https://www.gate.com/share/cbblaxit)|
| Gate永续USDT|gtc|永续合约|20%|[注册账户](https://www.gate.com/share/cbblaxit)|
| KuCoin现货|kc|现货|---|[注册账户](https://www.kucoin.com/)|
| KuCoin永续USDT|kcp|永续合约|---|[注册账户](https://www.kucoin.com/)|
| KuCoin永续USDC|kcc|永续合约|---|[注册账户](https://www.kucoin.com/)|
| BitGet现货|bg|现货|20%|[注册账户](https://partner.bitget.com/bg/cbbla)|
| BitGet永续USDT|bgu|永续合约|20%|[注册账户](https://partner.bitget.com/bg/cbbla)|
| BitGet永续USDC|bgc|永续合约|20%|[注册账户](https://partner.bitget.com/bg/cbbla)|
| HyperLiquid永续USDC|hpc|永续合约|---|[注册账户](https://app.hyperliquid.xyz/)|
| HashKey现货香港|hk|现货|---|[注册账户](https://www.hashkey.com/)|
| Backpack现货|bp|现货|---|[注册账户](https://backpack.exchange/)|
| Backpack永续USDC|bpc|永续合约|---|[注册账户](https://backpack.exchange/)|
| Aster现货|at|现货|10%|[注册账户](https://www.asterdex.com/zh-CN/referral/301896)|
| Aster永续USDT|atc|永续合约|10%|[注册账户](https://www.asterdex.com/zh-CN/referral/301896)|
| Lighter永续USDC|ltc|永续合约|---|[注册账户](https://app.lighter.xyz/)|


