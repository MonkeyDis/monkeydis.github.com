# Android学习笔记之——初识Android

从今天开始断断续续记录我在学习Android过程中的一些总结、想法以及疑惑，希望与大家一起学习进步，同时也希望大家监督。

### Android程序结构
/res 这个目录下面是各种资源
+/layout 程序的界面、布局
+/values 一般是记录字符串资源，可以有多个values文件夹，对应不同的语言
+/drawable 程序用到的图片资源（包括程序Icon）

上面的几个文件夹里面所定义的东西，都会在R.java文件中找到对应的ID，我们在代码中就可以通过引用R.java来访问我们所需要的资源。
R.java 文件是自动生成的，在/gen目录下面可以找到。
每当/res目录下有改动，R.java都会自动更新对应的ID。

### 几个基本概念
* View 界面元素。程序界面上面的所有元素(包括Button、MenuItem、TextView、EditText等等)，都是一个View。我们可以在Activity中通过R.java 中的ID找到对应的View。
* Activity 可以理解为程序逻辑的处理，类似于MVC中的Control层，可以控制View上面的元素，获取元素的值，并且可以绑定鉴定器，在监听器中处理程序逻辑。

今天就大概学了这么多，改天继续。

> Written with [StackEdit](https://stackedit.io/).