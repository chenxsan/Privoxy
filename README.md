Privoxy
=======

这是我自定义的 Privoxy 配置文件，包括以下文件：

文件名|作用
---|---
user.action|用户定义的 action 文件 
user.filter|用户定义的 filter 文件

# 用法

1. `cd` 到 Privoxy 的配置目录，比如 openSUSE 的 `/etc/privoxy/` 或 Mac OS 的 `/usr/local/etc/privoxy`
2. `mkdir else` 创建一个 `else` 目录
3. 如果有权限问题，请执行：
        sudo chown -R `whoami` else
4. `cd else`
4. `git clone https://github.com/chenxsan/Privoxy.git .`
5. 重启 Privoxy

## 规则共享

这些文件根据我个人浏览网页的习惯配置，不一定适用所有人。如有需要，请 fork 然后自定义。如果某些规则可共享，欢迎提 pull request。

## HTTPS 的情况

Privoxy 不支持 HTTPS 链接的过滤，推荐使用 [Greasemonkey](http://www.greasespot.net/) 一类工具。
