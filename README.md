# Privoxy 与奧黛麗·赫本

这是我的一个试验。

如果你不熟悉 Privoxy，那么你只要知道[它能替换 http 协议的图片](https://blog.zfanw.com/block-webpage-ad-with-privoxy/)就好。

这一条 Privoxy 规则非常简单：

```
{+block +handle-as-image +set-image-blocker{https://upload.wikimedia.org/wikipedia/commons/9/98/Audrey_Hepburn_screentest_in_Roman_Holiday_trailer.jpg}}
/.*\.(jpg|jpeg|png).*
```
这样，我就把所有 http 协议的图片都替换成奧黛麗·赫本，在浏览器上访问页面时，我会看到如下：

![赫本](images/replace-image-with-hepburn.png)

![赫本](images/replace-img-with-hepburn.png)

这意味着什么？这意味着，这些站点的图片还在使用 http 协议，而不是 https。

## 图片提交

如果你也使用 Privoxy，欢迎试用前面的规则，也欢迎提交有趣的图片。

## 图片许可说明

关于图片使用许可，请见 [Wikipedia 说明](https://upload.wikimedia.org/wikipedia/commons/9/98/Audrey_Hepburn_screentest_in_Roman_Holiday_trailer.jpg)。