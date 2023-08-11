---
title: 在国内环境下申请Freenom免费域名
subtitle: Freenom下域名申请
date: 2022-07-04 15:21:07
authors: [RamSong]
tags: [域名,Freenom,白嫖]
images: [https://ramblog-gh.imgix.net/Post/Blog/2/hub.jpg]
featuredImage: "https://ramblog-gh.imgix.net/Post/Blog/2/hub.jpg"
description: 通过Freenom申请tk.ml.cf.ga.gq后缀的免费域名,对于想低成本搭建网站或测试项目,申请Freenom的域名还是很有必要的。
---
通过Freenom申请tk.ml.cf.ga.gq后缀的免费域名,对于想低成本搭建网站或测试项目,申请Freenom的域名还是很有必要的。
<!--more-->

<iframe src="https://player.bilibili.com/player.html?aid=635443680&bvid=BV1zb4y1n7sX&cid=476068315&page=1" allowfullscreen="allowfullscreen" width="100%" height="500" scrolling="no" frameborder="0" sandbox="allow-top-navigation allow-same-origin allow-forms allow-scripts"></iframe>

# 要求

1.一个能访问网页的设备

2.一个IP 和 与IP地址对应的 **真实** 个人资料

3.一个邮箱

（主要是注册 Freenom账号 和 CloudFlare账号 ）

# 前言

  **[Freenom](https://www.freenom.com/)自称是世界上第一个也是唯一的免费域名提供商。 它们说它们的使命是把互联网带给世界人民，帮助各国发展自己的数字经济。**

:::default
官网介绍
:::
![](https://ramblog-gh.imgix.net//Post/Blog/2/abfreenom.png)

  对于想低成本搭建网站，或者搭建一些测试项目，那么使用一个低成本的域名乃至免费的域名还是很有必要的。

  平台一共有5个免费的顶级域名

```
 .tk 域名是南太平洋岛国托克劳的后缀, 
 .cf 域名是中非共和国的后缀, 
 .ml 域名是非洲国家马里的后缀, 
 .ga 域名是加蓬国家顶级域名后缀, 
 .gq 域名是赤道几内亚国家地区后缀。
```

# 环境准备

##   Why？

  Freenom的验证使用的是 Google 的 ReCAPTCHA ，由于国内 GFW 的功劳，ReCAPTCHA 无法在国内使用（特供版，镜像源除外）

  但是 Freenom 的购买需要 ReCAPTCHA 的参与，So我们需要把 ReCAPTCHA（[google.com/recaptcha](https://google.com/recaptcha)）重写到 ReCaptcha 国内镜像（[recaptcha.net/recaptcha](https://recaptcha.net/recaptcha)）上

##   插件安装

  浏览器重写插件有很多，这里使用 [Header Editor](https://he.firefoxcn.net/)

| 浏览器                                                       | 安装                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![Firefox Logo](https://cdn.staticfile.org/browser-logos/58.1.3/firefox/firefox_16x16.png) Firefox | [Mozilla Add-on](https://addons.mozilla.org/en-US/firefox/addon/header-editor/) 或 [Github自分发版本](https://github.com/FirefoxBar/HeaderEditor/releases) |
| ![Chrome Logo](https://cdn.staticfile.org/browser-logos/58.1.3/chrome/chrome_16x16.png) Chrome | [Chrome Web Store](https://chrome.google.com/webstore/detail/header-editor/eningockdidmgiojffjmkdblpjocbhgh) |
| ![Edge Logo](https://cdn.staticfile.org/browser-logos/58.1.3/edge/edge_16x16.png) Edge(Chromium) | [Chrome Web Store](https://chrome.google.com/webstore/detail/header-editor/eningockdidmgiojffjmkdblpjocbhgh) |

  我这里下了个 [crx文件](https://gcdn.ramsong.cn/bilibili/Freenom/Header%20Editor_v4.1.1.crx)

## 规则写入

  点击插件，进入管理界面，依次点击-导出与导入-下载规则-保存

  规则  https://gcdn.ramsong.cn/bilibili/Freenom/GoogleRedirect.json

![](https://ramblog-gh.imgix.net//Post/Blog/2/cha-set.png)

   之后保持规则启用即可

![](https://ramblog-gh.imgix.net//Post/Blog/2/cha-hub2.png)

# 域名选择

  打开 Freenom 官网 https://www.freenom.com/

  随便输入一个域名，建议加上后缀(xxx.tk/ml/ga/cf/gq)，否则可能**无法选择**，网页有Bug。

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-g.png)

  这里随便输入了一个域名，直接点击完成

  这边可以看到右下角谷歌的 ReCAPTCHA 协议已经出来了

  接着我们选择时间，调为12个月

  （12个月免费，1年9.95USD，........）

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-xuan.png)

  点击 **Continue** 进入下一步

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-you.png)

  来到这个界面，在这输入邮箱后会有一封验证电子邮件发给你

  ++有些邮箱发送不了，换一个就可以了++

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-yanmail.png)

  点击这封邮件来到注册界面

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-ziliao.png)

  ==可以使用各种信息生成器==

:::warning
填写信息的地址务必要与你现在的IP归属地相符
:::

  然后点击下一步

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-shenok.png)

  出现这个就代表你的域名申请成功了

# 域名转移

##   简介

  由于 Freenom 自带的解析系统太 ”厉害“ 了，所以我们需要使用其它解析商进行DNS解析。

  这里推荐两家， [DNSPOD（cn）](https://www.dnspod.cn/) 和 [CLOUDFLARE](https://cloudflare.com/) 。

  DNSPOD 已经被腾讯收购，二次加工后，DNSPOD的速度也不错，特别是在国内，但由于是腾讯经营，所以注册要手机号，解析好些也要实名，国际版我没用过......

  CLOUDFLARE 是全球最大的DNS解析商，并且提供免费的CDN和防御等，反正很nb，注册也很简单，仅需邮箱账号......

## 实操  

  这里使用CLOUDFLARE进行演示

  打开 [CLOUDFLARE 官网](https://cloudflare.com/)  ，注册过程不再演示，进入主页面后，点击添加站点

![](https://ramblog-gh.imgix.net//Post/Blog/2/cloudflare-add1.png)

输入你的域名，添加。

![](https://ramblog-gh.imgix.net//Post/Blog/2/cloudflare-add2.png)

选择免费计划（当然你有钱当我没说）

![](https://ramblog-gh.imgix.net//Post/Blog/2/cf-xuan.png)

之后一路继续来到这个界面

![](https://ramblog-gh.imgix.net//Post/Blog/2/cf-fuzhi.png)

现在返回 [Freenom](https://www.freenom.com/) 点击顶部的 Servies-My Domain 

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-gai1.png)

点击你需要管理的域名右边的 Manage Domain，进入这个界面

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-gaiguan.png)

选择 Management Tools - Nameservers

![](https://ramblog-gh.imgix.net//Post/Blog/2/freenom-dns.png)

  把 CLOUDFLARE 给的 DNS地址 填进来就可以了

  然后就是漫长等待，成功之后cloudflare会给你发*邮件提醒*

  域名这样显示就代表成功了

![](https://ramblog-gh.imgix.net//Post/Blog/2/domainok.png)

  之后你就可以**自由解析**了

# 链接汇总

Freenom：https://www.freenom.com/

Cloudflare：https://www.cloudflare.com/

Dnspod : https://www.dnspod.cn/

Header Editor : https://he.firefoxcn.net/

规则：https://gcdn.ramsong.cn/bilibili/Freenom/GoogleRedirect.json