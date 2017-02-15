# RandomLayout
Android动画之随机摆放文字带飞入飞出效果

![](https://camo.githubusercontent.com/8374bc5b7feb5afd17c6c4962ae1ae8ca9ba2c00/687474703a2f2f61332e717069632e636e2f7073623f2f56313379796654393349326a676c2f716944526e355371636d44664f4d49576d5734766e526c354d413846572a7655525a6c775a692e38344355212f622f64427742414141414141414126626f3d62774747416741414141414346396b212672663d7669657765725f34)

# 随机布局类的介绍
## 静态

1. 随机大小,随机颜色
2. 布局随意 :
3. 控件和控件之间没有层叠
4. 控件没有超出屏幕

## 动态

1. 两个静态界面在切换
2. 有组合动画(alpha动画+scale动画)

## 实现:口述

## 相关类介绍

- AnimationUtil:生成组合动画的工具类
- RandomLayout:生成随机布局
- StellarMap:里面有两个随机布局,控制它的切换效果
    - 用来管理两个随机的布局RandomLayout
	- 设置数据的方式：setAdapter(),
	    - getGroupCount() : 有几组数据
	    - getCount（Group）:第几组数据的个数
	    - getView(group,position)

- ShakeListener:摇一摇工具类