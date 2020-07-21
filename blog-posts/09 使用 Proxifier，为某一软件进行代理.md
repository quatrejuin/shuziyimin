# 09 使用 Proxifier，为某一软件进行代理

因为 Google 的 backup & sync Mac 版本无法自定义socks代理，尝试了两种方法。

## 一：\~\~该方法不推荐：使用 shadowsocksx-ng 的 http 代理\~\~

shadowsocksx-ng 使用 munual mode/ 手动模式 同时开启 http 代理
在系统设置中更改为 https代理，并使用shadowsocksx-ng 中的 http 端口
能够登录Google drive 的 Mac 版本（ backup & sync），但同步数据十分不稳定。
故换用方法二。

<!-- more -->

## 二：使用 [Proxifier](https://www.proxifier.com/) 针对某一软件进行代理

**0. 简介**

Proxifier 作为一款网络代理软件，可以针对某一款软件设置特定代理规则。虽然 shadowsocks 可以自定义规则，但是遇到某些软件，像 Google drive 的 backup & sync 不支持 socks 代理的，就只能使用 proxifier 进行配置了。具体原理可以参考数码荔枝写的[文章](https://www.lizhi.io/review/74314755)。

Proxifier 虽然强大，但是使用十分简单。

- Proxies 用来添加代理服务器，可以添加 proxy chains 用来均衡负载。
- Rules 即 设置规则，为某一款软件的或某一网址进行配置，如果手动配置，记得把shadowsocks 之类的代理软件设置为直连，避免代理无限循环。
- DNS 建议选择使用 **Resolve hostnames through proxy** ， 即使用代理服务器的DNS，避免 DNS 污染。

![](media/15273082804441/15273083348232.jpg)




**1. 下载 Proxifier**
[Proxifier官网](https://www.proxifier.com/) ，有 Windows 版本和 MacOS 版本。

**2. 购买**
付费软件，可以免费试用一个月。官网卖的较贵，[数码荔枝的淘宝店](https://item.taobao.com/item.htm?id=535723275520) 有售正版，150元左右。

**3. 安装并导入规则**

[Github](https://github.com/Jamesits/proxifier-profiles) 上已经有写好的规则，直接将其中的 Current.ppx 文件下载并导入到 *\~/Library/Application Support/Proxifier/Profiles* 即可。

具体规则大概有：
- 常用代理软件直连避免代理无限循环
- 本地直连
- 常用管理路由器地址直连
- P2P下载直连
- 中国站点（使用熊猫翻滚的规则）直连
- 常见被封网站代理
- 不稳定的服务（包括iTunes，iCloud，**Mac App Store** 微软服务，GitHub等）代理

具体查看 项目的 readme ， 同时可以根据自己需要进行修改

导入配置文件后，重新打开 Proxifier 即可在程序中切换配置文件。

![](media/15273082804441/15273083492058.jpg)




**4. 自定义规则**

- 代理服务器 (Proxies)：需要与 shadowsocks 的本地端口一致，默认是127.0.0.1:1080；如果使用的是shadowsocksx-ng，就需要更改为 127.0.0.1:1086
- 规则 (rules)：增加 backup & sync，其他规则根据个人需要进行更改

![](media/15273082804441/15273083627648.jpg)

- 注意：Mac app store 和 微软 等不稳定的服务也是使用代理，如果流量有限，注意更改


