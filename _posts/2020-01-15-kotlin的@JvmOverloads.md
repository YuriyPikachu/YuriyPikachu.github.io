---
layout:     post
title:      kotlin的@JvmOverloads
subtitle:   kotlin的@JvmOverloads会不会生成多余的方法
date:       2020-01-15
author:     Yuriy
header-img: img/post-bg-rwd.jpg
catalog: true
tags:
    - 源码
    - kotlin
---

## kotlin的@JvmOverloads会不会生成多余的方法
进行代码review的时，新同事在kotlin方法上用了@JvmOverloads注解，说是为了兼容java代码，听了下表示了解。但他说该注解不会生成多余的java方法，我当时对这点心存疑虑，所以最近有时间正好验证下。

### 没加@JvmOverloads的Demo
<img src="https://tva1.sinaimg.cn/large/006tNbRwly1gayf5see85j30ec04xjrd.jpg"/>             

#### 该Kotlin 生成Java代码
<img src="https://tva1.sinaimg.cn/large/006tNbRwly1gayf5s9o16j30pu0apmxl.jpg"/>

### 加@JvmOverloads的Demo
<img src="https://tva1.sinaimg.cn/large/006tNbRwly1gayf5s49klj30ea0543yj.jpg"/>

#### 该Kotlin 生成Java代码
<img src="https://tva1.sinaimg.cn/large/006tNbRwly1gayf5rwk5tj30q90gqgmp.jpg"/>

了解更移动开发知识，欢迎关注公众号：
![](https://tva1.sinaimg.cn/large/006tNbRwgy1gayiubsiuaj309k09kdfn.jpg)         
* 头条：[Android开发加油站](https://www.toutiao.com/c/user/1789857904/#mid=1581788092440589)
* 微博：[Android开发加油站](http://weibo.com/2648402234/profile?rightmod=1&wvr=6&mod=personinfo&is_all=1)
* QQ技术交流群：389274438
* 博客：[https://YuriyPikachu.github.io](https://YuriyPikachu.github.io)
* 简书：[YuriyPikachu](https://www.jianshu.com/u/1df4d713a12c)
* csdn：[YuriyPikachu](https://blog.csdn.net/pjingying)
* github：[https://github.com/YuriyPikachu](https://github.com/YuriyPikachu)
* 邮箱：[YuriyPikachu@163.com](YuriyPikachu@163.com)
