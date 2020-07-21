# 14 在中国如何使用 Apple News？

本文更新于2019年5月日。如果您需要了解 Apple News+ 相关信息，文章稍后会发出，欢迎通过 [RSS](https://digitalimmigrant.org/feed) / [Twitter](https://twitter.com/shuziyimin) / [Telegram Channel](http://t.me/shuziyimin) 订阅更新。
<!-- more -->

# Apple News 简介
Apple News 是苹果在 iOS 和 macOS （10.14及之后的版本）设备上自带的新闻软件。目前仅在美国、英国和澳大利亚运营。它不生产内容，只搭建平台聚合新闻，比起 Google News, Feedly, Yahoo News 等平台，最大的区别在于，Apple News 需要内容发布者主动将内容发布在 Apple News 上，而不是像其他平台通过算法抓取。统一的格式样式保证了阅读体验。同时，使用 Apple News 时，内容发布者无法通过各类 tracker 向你定向推送广告。

![digital\_immigrant\_14\_Apple-News-Screenshots](https://cdn.shuziyimin.org/blog-14-4-1564981790.png)



上图是 Apple News iPhone 老版本的样式。
只有三栏, Today 一栏，混合了头条新闻，热门，个性化推荐，视频专区等等。也即是**智能推荐**和**热门内容**的合集
第二栏 Spotlight 是**编辑推荐**的内容，人工推荐在聚合类新闻软件中并不多见，典型的苹果作风。
第三栏 Browse 是**个人关注**，可以是各大内容提供方，也可以是某个话题。


# 破解原理
**非中国大陆地区**
Apple News 虽然在很多国家地区未提供服务，但设备上若使用美区 Apple ID 登陆，或者设置中地区更改为美国，Apple News 即可使用。如你在非中国大陆地区，只需要在 iOS 上切换 iTunes 账号/ 地区即可使用 Apple News。 

**中国大陆地区**
中国大陆地区比较特殊，Apple News 会识别设备的IP 地址，移动运营商等信息，来限制中国大陆地区用户使用。这应该是已知的苹果对自己服务作出的最严格的地域限制。

在iOS 设备使用 Apple News，需要 **1**: iTunes中使用美区Apple ID； **2** 设置中地区切换为美国； **3** IP 地址为美国/英国/澳大利亚等运营区域； **4** 使用非中国运营商/开启飞行模式 。
在 macOS 设备上使用 Apple News 需要 **1** 设置中地区切换为美国；**2** 网络 IP 地址是美国/英国/澳大利亚等运营区域

如果你觉得麻烦，欢迎使用 [Google News](https://itunes.apple.com/us/app/google-news/id459182288?mt=8) 或者 [Feedly ](https://itunes.apple.com/us/app/feedly-smart-news-reader/id396069556?mt=8)， 内容源没差，就是丑了点，又不是不能用🌚。


## iPhone/iPad 设备上使用 Apple News

**第一步：在主屏上显示 Apple News**

-  iTunes & App Store 账号更换为美区
-  设置- 通用- 语言/地区 中，切换地区为美国

这里需要介绍一下 Apple ID，iOS 上登陆的 Apple ID (苹果账号) 一般用于两种服务。一是 iCloud 文件及系统安全，二是用于 iTunes & App Store等购买服务。

在 iOS 的设置中 退出  iTunes & App Store 的登陆，换成[美区 Apple ID](https://digitalimmigrant.org/171)，Apple News, Apple TV 等软件就会出现在设备上了。

**第二步：正常使用 Apple News**

完成第一步，你在几乎所有国家都可以正常使用 Apple News 了。仅仅中国特殊，不但检测 IP地址，若发现 MCC ([移动设备国家代码](https://en.wikipedia.org/wiki/Mobile_country_code)) 是中国，则提示无法在地区使用。

在 iPhone 上需开启飞行模式。打开 Wi-Fi，使用 VPN 或者[SS类软件](https://shadowsocks.org/en/index.html)的全局代理。iOS 上，Apple News 对代理的 IP 没有特别限制，但建议使用主运营区域的。**但必须开启飞行模式这一点，等于屏蔽移动网络，代价很大且不具有普适性。** 

若在没有插 SIM卡的 iPad 上，使用 VPN 或者SS类软件的全局代理即可。常在Wi-Fi网络下扔着的 iPad 更适合用来阅读新闻等。

**第三步：Trouble Shooting**
如果按照上述步骤一步一步操作仍不可用，或者本来可用，突然不可用。可以尝试在 设置中搜索 "Location" 选择 “Reset location and privacy"，这样可以重置对所有 APP 及服务的授权，重新打开 News 时关闭地理位置授权即可。

如果是购买国内常用的 SS 代理服务，部分美区节点可能没有被苹果识别为美国，多切换几个节点尝试。



## Mac 设备上使用 Apple News

**第一步：在主屏上显示 Apple News**

![digital\_immigrant\_14\_google-news-screenshots02](https://cdn.shuziyimin.org/blog-14-2-1564981788.png)


macOS 需升级到10.14 macOS Mojave。MacOS 上仅需要在 系统设置-语言与地区 中将地区更改为 美国，Apple News 就会出现在应用页面。若仍未出现，可以在 应用程序 中查看到，按住拖到 dock 栏方便使用。

![digital\_immigrant\_14\_google-news-screenshots03](https://cdn.shuziyimin.org/blog-14-3-1564981789.png)


**第二步：正常使用 Apple News**
点开 Apple News， 很可能会提示该地区不支持。使用 VPN 或者[SS类软件](https://shadowsocks.org/en/index.html)的全局代理。更换代理后，双击dock 上的 Apple News 选择关闭，然后打开即可。若经常使用全局代理不方便，也可以考虑使用 [Proxifier ](https://digitalimmigrant.org/44)针对电脑上的每个软件分别设置代理策略。

如果是 Surge 用户，开启增强模式后，增加针对 News 的进程代理美国IP地址即可。如果是其他代理软件，觉得全局代理的体验较差，可以新增规则，将 `apple.news` 域名设置为Proxy，将 `apple.comscoreresearch.com` 设置为 Deny。 

注意，与iOS不同，macOS 上对 IP 地址还是有要求的，若使用加拿大或者其他非 Apple News 运营地区的 IP地址，仍会显示为该地区不支持。

**第三步：Trouble Shooting**
如果是购买国内常用的 SS 代理服务，部分美区节点可能没有被苹果识别为美国，多切换几个节点尝试。

如果仍有问题，建议邮件联系 [hi@shuziyimin.org](hi@shuziyimin.org) 以获得最快速的回复。 


# 不想那么折腾怎么办

总结来看，iPhone 上使用的缺点是必须要禁用移动网络；iPad 使用的缺点是不方便到处携带；Mac 上配置成本也不低。Google News 在今年2018年迎来一次大改版，在使用和内容上，毫不逊色 Apple News，只是 [Google News](https://itunes.apple.com/us/app/google-news/id459182288?mt=8) 会直接打开原网页链接，字体大小排版各具特色，没有 Apple News 统一发布看起来讨人喜欢。

# Apple news 与 Google News 对比

![digital\_immigrant\_14\_google-news-screenshots](https://cdn.shuziyimin.org/blog-14-4-1564981790.png)

| App | Tab 1  | Tab 2 | Tab 3 | Tab 4 |
| :-- | :-- | :-- | :-- | :-- |
| Apple News | 智能推荐+热门内容 | 编辑推荐 | 自选话题/内容提供方 | 无 |
| Google News | 智能推荐 | 热门内容 | 自选话题/内容提供方 | 浏览话题/内容提供方 |


由上可见，Google News 没有人工的「编辑推荐」，Apple News 因为对内容提供方门槛较高，比Google News 的更少些，除此之外，在内容上没有差异。


# 在 Apple News/ Google News 上看什么？

这个展开讲内容就会超级多了。欢迎参考本博客的另外几篇文章，看欧美电视电影版图，虽然偏向于电视电影，但是也可以帮你更好了解各个媒体的立场。同时还有获取资讯的 APP 也有一些推荐。

本文会持续更新。





