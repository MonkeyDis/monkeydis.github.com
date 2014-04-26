---
layout: post
title: Android学习笔记之——近日小结
---

# {{page.title}}

<p class="meta">2014-04-10 23:29:10 珠海</p>

今天一口气看完了一个简单的[游戏开发入门视频](http://www.howzhi.com/course/7022/?ref=cbc "数独游戏开发")，虽然视频略挫，但还是重新帮助我梳理了一下项目的基本元素、流程。  
现在尝试来整理下学习至今学到的一些东西吧~  
* View（视图）
** 界面上看到的元素基本都是View，Button、TextView、ProgressBar等等都是View的子类，这些都是单个的组件；
** ViewGroup也是View的子类，ViewGroup可以理解为集合，其子类有各种Layout，还有一些已经实现好的组件，例如DatePicker、TimePicker
** 我们可以通过继承View类，重载onDraw()方法来实现自己的View  
具体是通过Canvas，在上面绘制自己想要的图形、文字、图片等
* Activity（活动）
** Activity应该负责程序逻辑
** 一个Activity对应于程序的一个主界面，处理这个界面下的点击事件、数据计算等
* Intent（意图）
** 通过Intent，我们可以控制不同界面之间的跳转
** 在Intent里面包装数据，用来在不同的界面(Activity)之间进行数据共享
上面是程序主体的基本结构。分别构成了程序的视图层、数据层和控制层。


另外，还有其他的程序组成元素：
* AndroidManifest.xml
** 程序清单，对程序的基本描述，包括如下内容：
*** 版本号
*** 程序名
*** 支持的SDK
*** 需要的权限
*** 支持的设备屏幕大小
*** ……
** 程序中用到的所有Activities必须都在这里声明，否则程序运行中会抛出找不到Activity的异常（）
* res
** res文件夹下是所有用到的资源文件，包括：
*** layout/，布局文件，一般一个Activity会对于一个layout文件
*** drawable*/，图片文件
*** values/，字符串资源、以及程序中可以用字符串表示的一些值（比如颜色的RGB值）
*** ……
** res文件夹下的所有资源，都会在R.java文件（自动生成的）中有一个唯一对于的ID，我们在源代码中可以通过这些ID引用到对应的资源




P.S  上次说的Sublime Text 2输入中文会闪屏的问题，在我关机重启后就不重现了…… 看来是第一次安装完有点问题。