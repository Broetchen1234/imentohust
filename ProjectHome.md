Mentohust的iOS版，iOS锐捷认证客户端，支持在iOS设备(iPhone/iPad/iPod Touch)上直接登陆锐捷，彻底告别开PC作wifi中转的日子，不再需要connectify、不再需要刷各种路由，让iOS和windows一样直接登录锐捷。

# 前提 #
  * iPhone/iPad／ipod touch必须已越狱。
  * 无线路由作为HUB使用，即入口网线不要接WAN口，而应该接LAN口，同时需要关闭路由器的DHCP服务器功能。最好先用PC机测一下能否通过WIFI登录锐捷。

# 安装方法 #
程序包括两部分必需分别安装，从Downloads里下载安装包：

  * 前端的登录界面，是一个ipa包，使用一般的方法安装（iTunes/iTools等皆可）
  * 另一部分为后台服务iMentoHUST Daemon, 为deb包，推荐用iFile或命令行dpkg安装，其他的方法（如iTools）可能安装不上。装完后最好重启一下设备。

# 设置 #
  * 从1.2版起dhcp、组播地址等设置移到了系统的 设置->应用程序->iMentoHUST 中。
  * 从1.2版起可以使用mpf认证数据文件，命名为custom.mpf用iTunes上传到本应用目录下，并打开设置中的"启用自定义数据文件"开关即可。

# 一些问题 #
> 请使用最新版本，并作正确的设置，可解决大部分认证失败问题。
  * 若登录时卡在“正在寻找认证服务器..”，那么尝试一下先断开再重新登录。
  * 必须先连上wifi（最好在wifi设置中将其它搜到的wifi接入点忽略，以免自动切换接入点）。
  * 若提示"动态ip地址绑定错误"，请在设置选择合适的DHCP方式。
  * 若提示"不允许使用的客户端类型"，请用[MentohustTool](https://code.google.com/p/mentohust/downloads/detail?name=MentoHUSTTool.7z&can=2&q=) 抓包得到mpf数据文件，并命名为custom.mpf，用iTunes上传到本应用目录下,并打开设置中的"启用自定义数据文件"开关即可。
  * 若上述方法都无法解决问题，发请按本程序界面右上角的i图标，将日志窗口的内容发到https://code.google.com/p/imentohust/issues/list,

# 相关 #
[mentohust](http://code.google.com/p/mentohust/)