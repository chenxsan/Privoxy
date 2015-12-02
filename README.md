Privoxy
=======

这是我自用的 Privoxy 配置文件，主要包括两个文件：

1. user.action
2. user.filter

# 用法

1. `cd` 到 Privoxy 的配置目录， 

    * openSUSE: `/etc/privoxy/` 
    * Mac OS: `/usr/local/etc/privoxy`
2. `mkdir else` 创建一个 `else` 目录
3. 新创建的 `else` 目录通常会有权限问题，请执行：

        sudo chown -R `whoami` else
    将 `else` 目录所有者修改为当前用户。
4. `cd else` 切换到 `else` 目录
4. `git clone https://github.com/chenxsan/Privoxy.git .` 将配置文件克隆一份到 `else` 目录
5. 打开 Privoxy 的主配置文件 `config`，在文件最后添加以下两行：

    ```
    actionsfile else/user.action
    filterfile else/user.filter
    ```
5. 可能还需要重启 Privoxy
6. 往后更新此配置文件只需要进入 `else` 目录执行 `git pull`

## 规则共享

这些文件根据我个人浏览网页的习惯配置，不一定适用所有人。如有需要，请 fork 然后自定义。如果某些规则可共享，欢迎提 pull request。

## HTTPS 的情况

Privoxy 仅支持 HTTPS 链接 [host 部分的过滤](http://www.privoxy.org/faq/misc.html#AEN909)，需要更细的定制的话，推荐使用 [Greasemonkey](http://www.greasespot.net/) 一类工具。

## 效果

1. 在土豆看银魂动画基本不会碰上视频广告
