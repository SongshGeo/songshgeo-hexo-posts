---
title: 使用RSS订阅信息源
categories: 日渐
author: Shuang (Twist) Song
tags:
  - 读书
  - 地理
summary: 如何使用RSS系统应对这个信息爆炸的时代？
toc: true
date: 2021-08-08 20:33:36
img: 'https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/xFOcKQ.png'
---

在这个信息爆炸的时代，应该很多人有这样的需求：

- 及时追踪不同信息源的更新
- 集中时间和地点浏览信息源
- 摆脱平台推荐算法的干扰
- 方便收藏、归类、回溯看过的信息

对于这些问题，我的终极解决方案就是：**RSS**系统。

在被很多人偷窥过屏幕后（bushi），发现周围很多小伙伴都很喜欢我为自己打磨的信息源订阅系统，咸来问讯。所以今天详细介绍一下。

首先展示主要界面：

![Reader的主界面](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/931CA2.jpg)

在这个系统里，我利用**RSS订阅**的方式将所有感兴趣的**信息源**汇总到一起，并分为四类：

- Info：知识、信息类信息源。
- Stories：故事、非虚构写作相关的信息源。
- Updates：软件、榜单、实验室、大学官网、展览的最新动态。
- Users：有高质量片单/书单的豆瓣用户、关注的学者主页。

可见，RSS的订阅源是多种多样的，因为RSS诞生之初就旨在让用户以聚合的方式从多渠道快速订阅获取信息：

> RSS广泛用于网上新闻频道，blog和wiki，主要的版本有0.91, 1.0, 2.0。使用**RSS订阅**能更快地获取信息，网站提供RSS输出，有利于让用户获取网站内容的最新更新。网络用户可以在客户端借助于支持**RSS的聚合工具软件**，在不打开网站内容页面的情况下阅读支持RSS输出的网站内容。

根据我的经验，搭建属于自己的RSS系统有三步：

- 找到适合自己浏览的信息源
- 为想要浏览的信息源找到RSS订阅
- 合理使用聚合工具软件

## 找到信息源

找到信息源在现在似乎不是什么难事，可能很多人已经习惯了随手把看到的好信息源加到收藏或关注列表。但在RSS系统中最好不要这么干，我建议你的信息源一定是要经过严格过滤筛选的。两年前我刚开始使用RSS系统时，中间曾一度放弃，因为我把所有想浏览的东西都塞到了RSS里，导致每次打开软件都会看到几百个未读消息，带来极大的阅读压力。

譬如最初我把所有follow的学术期刊也使用RSS订阅了，后来发现每天都产生大量的垃圾消息，在其他更轻松的信息源（如报纸和新闻）面前，这些学术期刊的更新似乎也不那么吸引人，导致读新闻的时候有负罪感，读文献又读不进去。而且，学术期刊本有更专业的软件去管理和追更，为什么要加进来污染我的RSS系统呢。

所以找订阅源的时候，建议大家先问自己这样一个问题：

>我会在何时何地以何目的浏览RSS？

我的回答是，我会抽出**每天一个小时**左右的时间，在**笔记本电脑**上，目的是**找到值得进一步关注的主题或信息**。

所以我找RSS的信息源有以下规则：

- 不需要立刻进行深度阅读（时间不允许），这意味着我不会在RSS追学术文献之类。
- 不需要追踪即时更新，这意味着我两三天不打开电脑，也不会有追更的压力。

## 找到RSS订阅源

有了想订阅的信息源后，下一步考虑如何找到信息源对应的RSS订阅源。

RSS的工作原理是将信息源的信息转化为可订阅的链接。有些网站本身就提供部分订阅链接，如豆瓣：

![豆瓣用户动态的订阅链接](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/FkrODF.jpg)

点进去后它会告诉你这是一个订阅源：

![订阅源格式](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/YxeIPD.jpg)

但是不是所有的网站都主动提供了RSS订阅源，所以大多数时候，如何找到合适的RSS订阅源都是一件让人苦恼的事情。这时候，程序员们可能就会想到自己生产一个订阅源，通过脚本爬取网页内容，生成RSS订阅源，再塞到自己的订阅列表里。

显然，这个“造轮子”的过程不适合大众用户，这时候就要借助开源的伟大力量了：RSSHub。

![RSSHub](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/xFOcKQ.png)

[RSSHub](https://docs.rsshub.app/)的口号是“万物皆可RSS”，这个开源社区里有一群程序员制作了各种奇奇怪怪网站的RSS源并共享，但凡是比较常见的信息源基本都能在RSSHub上找到合适的订阅链接。使用起来也很方便，只要安装浏览器插件，一旦你正在浏览的网站有RSS源，就会自动提示：

![RSS源的提示](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/np59oG.jpg)

利用这个方法，你可以做到：

- 订阅豆瓣/微博/B站用户的动态更新和收藏列表，看关注的人都在看什么好书或好片，以及他们写的推荐语（不需要关注用户，可以悄咪咪偷窥用户动态）：

![RSS追踪豆瓣用户动态的例子](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/khctbg.jpg)

- 订阅GitHub的各大awesome榜单，及时看有哪些亮眼的开源软件、算法或模型更新

![RSS追踪GitHub项目的例子](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/fAhtsE.jpg)

- 订阅自然基金委、你的大学、关注的实验室主页的最新动态：

![RSS追踪学术动态的例子](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/fReE75.jpg)

RSSHub还有更多奇奇怪怪的链接和玩法，可以自己探索。

这里值得一提的是，微信公众号在RSSHub上也有开源制作的链接，但因为反爬虫严格而常常失效。所以需要一个愿意维护稳定订阅源的程序员。所以用RSS订阅公众号，如果不想付费，那关注RSSHub的即时更新就可，只是它可能不大稳定。如果愿意付费，可以像我一样直接在淘宝上找了一个提供微信公众号RSS订阅的服务，提供服务的大佬会去稳定维护，价格也不贵...

![淘宝上订阅微信公众号的RSS源](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/f8iJBF.jpg)

## 合理使用RSS聚合软件

RSS订阅源只是一个链接，需要用聚合软件去管理这些源，Windows上的软件有很多，一搜一大把攻略，就不多说了。至于Mac系统，据我摸索Reeder应该体验最好的APP了。

![Reader的功能栏](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/gnRuWM.jpg)

它可以做到：

- 对感兴趣的文章星标，加标签，方便管理。
- 自动识别文章重点词句并加粗，节省浏览网页的时间，提升信息获取效率。
- 和各种你能想到的APP交互，分享发送到微信、电脑浏览器、手机浏览器、其他链接收藏工具等。
- 自动同步iCloud，而且是网页剪藏版本，哪怕网页链接失效，看过的内容也永不丢失。

## Other Tips

最后写几条合理使用RSS的小建议：

- 使用RSS的目的之一是打破互联网的“信息茧房”，需要经常去更新、淘汰、迭代你订阅的信息源。
- RSS只是管理信息来源的手段，从这些信息源收获怎样的信息，如何去管理这些收获，又是另一门课题，收藏本身不代表学习。
- RSS常用于快速浏览新闻，信息容易遗忘，碰到有用的信息需要及时打标签，以便在事后凭借一点点印象找到信息源回溯。
