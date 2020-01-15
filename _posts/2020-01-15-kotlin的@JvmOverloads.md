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
---

## kotlin的@JvmOverloads会不会生成多余的方法
进行代码review的时，新同事在kotlin方法上用了@JvmOverloads注解，说是为了兼容java代码，听了下表示了解。但他说该注解不会生成多余的java方法，我当时对这点心存疑虑，所以最近有时间正好验证下。

### 没加@JvmOverloads的Demo
<img src='https://github.com/YuriyPikachu/YuriyPikachu.github.io/raw/master/_posts/media/15790592349897/15790597042506.jpg' align='center' />

该 Kotlin 生成Java代码
<img src='https://github.com/YuriyPikachu/YuriyPikachu.github.io/raw/master/_posts/media/15790592349897/15790598944718.jpg' align='center' />

### 加@JvmOverloads的Demo
<img src='https://github.com/YuriyPikachu/YuriyPikachu.github.io/raw/master/_posts/media/15790592349897/15790599546708.jpg' align='center' />

该 Kotlin 生成Java代码
<img src='https://github.com/YuriyPikachu/YuriyPikachu.github.io/raw/master/_posts/media/15790592349897/15790600328783.jpg' align='center' />

