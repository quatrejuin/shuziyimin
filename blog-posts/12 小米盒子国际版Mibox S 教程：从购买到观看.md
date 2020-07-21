# 12 小米盒子国际版Mibox S 教程：从购买到观看

本文最后更新于2019年8月11日，有大量删减与改动。个人虽仍在使用小米盒子国际版，但精力有限，此文不再更新。本站其他文章仍会继续更新。
<!-- more -->

# 0. 简介
小米盒子国际版是小米在[美国](https://www.mi.com/us/mi-box-s/)、香港、台湾等地区发行的电视盒子。内置 Android TV，无开机广告。应用商店是 Google play, 安装软件无限制。两款均支持语音输入，Google assistance 提供服务。同时也是中国大陆可以用来看 Netflix 最便宜的设备之一，适合影音达人购买。

小米盒子国际版共有两代，MI BOX 和 MI BOX S。MI BOX 配置与 小米盒子3 类似，于2016年底发布，内置系统 Android TV  6，已可更新至 Android TV 8.0。MI BOX S 是前一代的升级款，配置与国内版 小米盒子4类似，于2018年底发布，内置系统 Android TV  8.1。

两款硬件配置差异不大，（毕竟小米盒子3 和4之间差异就不大）是完全没有必要换新的例行升级。两者最大的区别在于，MI BOX S 更像是一款针对国外市场发布的产品，进行了很多本土化的改进，比如遥控器进行了特别设计，有一键 Netflix 按钮。

# 1. 购买

-  香港小米之家：[分别在旺角和铜锣湾](https://www.mi.com/hk/service/mihome/)，售价469港币，即400元人民币左右。
-  香港丰泽：可在[丰泽官网](https://www.fortress.com.hk/zt/product/pfj4059hk-smart-tv-box/p/BP_11742093)查看哪些实体店有售；也可以线上预定，线下取货。价格与小米之家一致。百老汇和香港苏宁暂时没有销售。
- 淘宝代购港版。

# 2. 开机配置

开机需要登陆谷歌账户，一个可以科学上网的环境就十分有必要了。又因为刚开机连接 Wi-Fi 时无法设置 HTTP 代理，所以**只能通过路由器配置代理网络**。首次开机后可以安装 shadowsocks 安卓版，之后便无需使用路由器来进行代理。

**路由器使用开源固件配置代理**
华硕路由器等，略。

**使用 Surge 为路由器 进行代理**
[Surge](https://nssurge.com/) 是 MacOS 上的一款代理软件，提供强大的网关代理功能。若没有购置路由器的需要，可以使用 Surge 应付一下，Surge 是一款付费软件，但可免费试用30天。

- 下载安装，配置节点后将 Surge 设置为系统代理；并开启增强模式
- 将 Macbook 连入Wi-Fi，查看 Macbook 自动获取（DHCP）的 IP 地址 ，并查看路由器地址。按住 `Option` 键的同时点击桌面右上角状态栏 Wi-Fi 标志，即可查看到电脑 IP 地址与路由器 IP 地址。
- 将 Mac原先通过 DHCP 自动获取的IP地址 手动指定为固定 IP地址。
- 路由器设置中 DHCP 服务器，网关地址设置为 Macbook 的IP 地址；DNS服务器地址填写 198.18.0.2（Surge 默认，一般不变）。
- 完成以上步骤，所有连入Wi-Fi的设备都可以使用MacBook 上的代理网络了。

此处教程配图之后补上。

# 3. 必备软件
**必备软件：文件管理器**
更新：ES File Explorer 已被百度收购，[因为百度作弊](https://www.buzzfeednews.com/article/craigsilverman/google-play-store-ad-fraud-du-group-baidu)，导致所有海外软件均被 Google Play 下架，ES File Explorer 也不例外。

推荐使用 [FX File Explorer](https://play.google.com/store/apps/details?id=nextapp.fx&hl=en_US) 在电视版本商店找不到的话，可以在网页版本 Google Play 打开，登录同一 Google账号后，可以远程安装。通过文件管理器是安装 APK文件最方便的途径。
安装后，可以通过局域网向小米盒子转 APK文件，也可以把需要用的 APK 文件放在 Google drive 等网盘中，在 文件管理器中登陆 Google Drive 等网盘，下载文件安装。这里分享下我的[Google drive链接](https://drive.google.com/drive/folders/1w4sQ1jOFAz2MEevzcoscYf82u-52uCXw?usp=sharing)，可以直接转存。内有 Bilibili TV版，SS各版本。

-  Google drive 直接下载 APK 文件后点击安装，可能显示无法安装，再次下载点击安装即可。
- Bilibili 应该是官方提供的版本。
- shaodowsocks & shadowsocksR & obfuscation混淆插件；配置时可能需要鼠标来进行辅助操作。配置完成后，打开关闭使用遥控器即可完成。

**Spotify**
可从 Google play 下载，手机上登陆后，直接智能识别局域网内的其他设备，在电视设备上无需输入验证码等，直接点击确认即可进行账号同步，超级方便。

**Netflix**
Netflix and chill! 拿着遥控器躺在沙发上随意选美剧的感觉还挺不错。

若在路由器使用代理，路由器上的配置规则需要注意，尽量选择仅绕过中国大陆的规则，避免 Netflix 出错。
若是在电视盒子上使用代理软件，选择绕过中国大陆地址和局域网即可。
支持 Netflix 的代理请参考本网站的另一篇文章 [在中国看 Netflix，看这一篇就够了](https://digitalimmigrant.org/16)
如果需要看4K，折腾的就不少了

- Netflix 需要购买最贵的套餐
- 购买合适的代理，自建很难达到。
- 家中路由器性能需要足够，网线端口等也需要注意
- 电视 HDMI 端口和 HDMI连接线是否支持 HDCP 2.2 （High-Bandwidth Digital Content Protection），这部分可以参考[ Netflix 的官方解答](https://help.netflix.com/en/node/13444)。

# 4. 投屏播放
 投屏播放是经常会遇到的需求。如
 国内版小米盒子支持 DLNA AirPlay 等协议，但是小米盒子国际版仅支持 Chromecast 协议
 
**Chromecast 协议**
 Chromecast 协议是谷歌在android TV 上力推的协议，和 AirPlay 类似，根据[官网](https://www.google.com/chromecast/built-in/apps/)介绍，国际主流视频音频播放软件均支持此协议，试用体验也十分好。Mibox S 内置Chromecast，所以手机上YouTube Spotify等可以直接投屏，投屏后盒子负责解析链接进行播放，手机端可以充当遥控器进行控制，不影响手机上进行其他操作。
 
**DLNA 协议**
 [DLNA 协议](https://www.dlna.org/) 是intel 微软 索尼等于2003年建立的协议，2017年机构已解散，协议不再更新。国内视频软件如腾讯视频、爱奇艺等在投屏普遍使用 DLNA 协议，国内盒子也普遍支持 DLNA，所以没什么大问题。小米盒子国际版并不支持DLNA 协议，需要安装软件来支持。安装 ES File Explorer 后可以进行 DLNA 投屏。
  
 
# 5. Mi Box 的体验
**遥控器搜索功能**
按住遥控器语音键，对着遥控器说话即可搜索。小米盒子系统语言为中文情况下，能够准确识别中文和英文。如果已安装 Netflix 等流媒体软件，可以直接进行应用内搜索，在搜索结果中跳转到某APP，国内电视盒子也有这一类的功能，但是体验方面就较差了。

**Chromecast 功能**
YouTube，Netflix 等支持 Chromecast，直接投屏十分方便！ 


# 6. 升级
Mibox S 内置 Android 8.0，但因为小米在 8.0 上优化很差，盒子常出现待机后无法唤醒，或者蓝牙遥控器连接不正常，需要拔电重启来解决。这个问题目前依旧存在，如果因为无法接受这一点麻烦，建议不要购买 Mibox. 

小米盒子安装代理软件且设置全局代理后，实测依然无法下载系统更新。需要通过路由器等外部代理网络来完成系统更新。

