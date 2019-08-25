---
title: css-动画
date: 2019-08-12 07:04:08
tags:
photos:

---
## 一、动画定义
> **@keyframes(关键帧)规则:**
> from和to分别代表动画的开始点和结束点（分别可以用0%和100%来表示)
```
@keyframes 动画名称 {
	from{

	}
	to{

	}
}
```

```
@keyframes 动画名称 {
	25%{

	}
	50%{

	}
	100%{

	}
}
```
---

## 二、动画应用
> **1.指定关键帧的名称**
  animation-name: keyframename/none;


> **2.动画持续的时间（?s)**
  animation-duration: time;


> **3.动画延迟时间**
  animation-delay: time;


> **4.动画运动方向** 
  animation-direction: normal/reverse/alternate/alternate-reverse/initial/inherit;

值|描述
:--:|:--:
normal|默认值，动画按正常播放
reverse|动画反向播放
alternate|动画在奇数次（1、3、5...)正向播放，在偶数次（2、4、6...)反向播放
alternate-reverse|动画在奇数次（1、3、5...)反向播放，在偶数次（2、4、6...)正向播放
initial|设置该属性为它的默认值
inherit|从父元素集成该属性

> **5.动画结束后保留哪个样式**
  animation-fill-mode: none/forwards/backwards/both ;

值|描述
:--:|:--:
none|不改变默认值
forwards|保留最后一帧的样式
backwards|保留第一帧的样式
both|动画会在两个方向上扩展动画属性

> **6.动画播放的次数**
  animation-iteration-count: n/infinite;

值|描述
:--:|:--:
n|定义动画播放次数的数值
infinite|规定动画无限次数播放

> **7.动画执行的时间曲线**
  animation-timing-function: linear/steps(n)/ease/;

1. linear: 动画从开始到结束的速度是相同的。（匀速）   

2. steps(n,start/end): (作用于两个关键帧之间，而非整个动画)
    1. 把动画分成n步阶段性展示，n必须为整数。   

    2. start和end可选。指定在每个间隔的起点还是终点发生阶跃变化。
       * start：第一帧是第一步动画结束
       * end  ：第一帧是第一步动画开始

> **8.动画播放状态**
  animation-play-state: running/paused;

值|描述
:--:|:--:
running|动画播放
paused |动画暂停

> **9.速写**
  animation: duration timing-function delay iteration-count direction move_eye ;
 ---
## 示例（css3仿梦幻西游动画特效）

![-449598401.jpg](https://i.loli.net/2019/08/12/4Ksi8oQX7WRbayJ.jpg)
