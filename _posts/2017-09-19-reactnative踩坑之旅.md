---
layout:     post                    # 使用的布局（不需要改）
title:      react-native踩坑之旅              # 标题 
subtitle:   每日一踩                       #副标题
date:       2017-09-19              # 时间
author:     BY ldnjun                      # 作者
header-img: img/2017-09-04.png    #这篇文章标题背景图片
catalog: true                       # 是否归档
tags:                               #标签
    - ReactNative
---
**1. Super expression must either be null or a function, not undefined**
```javascript

```
**2. js中(),{}的区别

{ } 大括号， 表示 定义一个对象 ，大部分情况下要有成对的属性和值，或是函数 。

**3.mac打包安卓包遇到的问题

```
If you are using NDK, verify the ndk.dir is set to a valid NDK directory
```

mac没有安装ndk，安装步骤如下：

1.[下载ndk](https://developer.android.google.cn/ndk/downloads/index.html) 

2.解压压缩包 

3.配置环境 
```
vim .bash_profile

```
添加如下配置，这里的路径要写成自己ndk解压的路径
```
export PATH=${PATH}:/Users/julong/Downloads/adt-bundle-mac-x86_64-20140624/android-ndk-r16b

```

4.重启加载文件

```
source .bash_profile
```

5.测试是否成功

```
输入：ndk-build 
```
提示如下就成功了。
```
 *** Android NDK: Aborting    .  Stop.
```
