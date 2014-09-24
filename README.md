Privoxy
=======

Privoxy 配置文件


这是一份我自己使用的 Privoxy 配置文件库，包括以下文件：

1. config - 配置文件
2. user.action 
3. user.filter
4. easy* 系列文件

其中 easy* 列表根据[脚本](http://andrwe.org/scripting/bash/privoxy-blocklist)自动生成，[具体列表](https://easylist.adblockplus.org/en/)请根据自己情况补充，user.action 与 user.filter 用于个人定制一些规则。

## openSUSE 下用法

将 README.md 以外的文件下载拷贝到 /etc/privoxy/ 或 /var/lib/privoxy/etc/ 目录下即可。

## 关于规则的说明

规则是很隐私的东西，譬如我过滤有道词典的广告，就说明我经常用有道词典，这也是 AdblockPlus 这类工具的好处，通用，不暴露个人隐私，但因此它也就有了缺点，一些漏网之鱼顾不过来。这恰是定制的战场。但定制的话，规则太少，不通用。譬如我去除土豆网视频的广告，可能就只去了部分，因为这部分视频广告经常在我看的视频里出现，于是就被我逮到。

我个人来说，其实希望这份配置文件能有人提交 pull request，分享自己的过滤规则。Privoxy 是很小众的东西，一些小众的用户交流些规则，不伤大雅 - 只要稍稍注意保护下隐私就好。
