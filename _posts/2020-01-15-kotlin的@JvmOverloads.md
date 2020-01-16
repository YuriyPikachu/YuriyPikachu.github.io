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

