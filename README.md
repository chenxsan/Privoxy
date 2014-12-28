Privoxy
=======

这是我自用的 Privoxy 配置文件库，包括以下文件：

文件名|作用
---|---
config|配置文件
user.action|用户定义的 action 文件 
user.filter|用户定义的 filter 文件
easy* 系列文件|脚本生成的 action/filter 文件

easy* 列表是根据[脚本](http://andrwe.org/scripting/bash/privoxy-blocklist)自动生成，[具体要用哪些](https://easylist.adblockplus.org/en/)请根据自己情况补充或删减。

## openSUSE 下用法

1. 下载配置文件
2. 将它们拷贝到 _/etc/privoxy/_ 或 _/var/lib/privoxy/etc/_ 目录
3. `sudo rcprivoxy restart` 重启 Privoxy

## 规则的说明

根据我个人习惯配置的，不一定适用所有人。如有需要，请 fork 然后自定义。如果某些规则可共享，欢迎提 pull request - 不过请保护自己的隐私，别把某些耻感很强的网址发出来。
