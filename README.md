Privoxy
=======

Privoxy 配置文件


这是一份我自己使用的 Privoxy 配置文件库，包括以下文件：

1. config - 配置文件
2. user.action 
3. user.filter
4. easy* 系列文件

其中 easy* 列表根据[脚本](http://andrwe.org/scripting/bash/privoxy-blocklist)自动生成，[具体列表](https://easylist.adblockplus.org/en/)请根据自己情况补充或删减，user.action 与 user.filter 用于个人定制一些规则。

## openSUSE 下用法

将 README.md 以外的文件下载拷贝到 _/etc/privoxy/_ 或 _/var/lib/privoxy/etc/_ 目录下即可。

## 关于规则的说明

根据我个人的习惯配置的规则，不一定适用所有人。如有需要，请 fork 然后自己定义。如果某些规则可共享的，欢迎提交 pull request - 不过请注意保护自己的隐私。
