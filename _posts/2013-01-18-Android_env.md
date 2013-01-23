---
layout: post
title: Android开发环境搭建
description: Android环境搭建步骤
categories: Android
tags: [HTML, input]
copyright: cn
---
# 1. 环境搭建前的准备
  搭建整个Android开发环境需要安装如下软件：JDK，Eclipse，Android SDK和ADT。  
  JDK：要求JDK 1.5+，建议JDK6.x 
  
  下载地址:http://www.oracle.com/technetwork/java/javase/downloads/index.html  
  
  Eclipse：Eclipse 3.4(Ganymede) or 3.5(Galieo)
  
  下载地址：http://www.eclipse.org/downloads 建议下载版本Eclipse IDE for Java Developers
  
  Android SDK:准确的说下载的不是SDK而是SDK的下载安装器，因为下载下来的并没有SDK，而是需要连接到官方网站下载所需要的SDK。
  
  下载地址：http://developer.android.com/sdk/index.html,选择windows平台进行下载。
  
  ADT：这是eclipse的一个插件，是在线安装的，下文会有介绍。
  
  所以，在搭建Android开发环境之前，需要确保已经下载了上述的安装包或者对应的软件已经安装了。

# 2. 环境的搭建

## 2.1. JDK安装
	 如果电脑中没有JDK的话，就安装已下载的安装包，安装时根据提示一步一步就行，设置环境变量步骤如下：
	 1、我的电脑->属性->高级->环境变量->系统变量中添加如下环境变量
	 2、JDK_HOME值为：C:\Program Files\Java\jdk1.7.0_10（JDK的安装目录）
	 3、CLASSPATH值为：.;%JAVA_HOME%\lib\tools.jar;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\bin;
	 4、Path：在开始追加%JAVA_HOME%\bin;
	 	 完成安装后，可以检查JDK是否安装成功。 
	 
## 2.2  Eclipse安装
   解压安装包即可使用。
## 2.3 Android SDK安装
   将下载的android_sdk_r18_windows.zip加压到任意路径（为了方便，尽量解压到eclipse所在目录）。
   运行SDK Setup.exe，如果网速好的话，可以把所有的Android版本都下载，另外最好将Tools和Extras也装上。
   如果有访问互联网的限制的话，可以直接从已经搭建过环境的同事那拷贝其SDK目录即可。对应的Android的版本在/platforms目录下。
   注意目录/add-ons和extras。
   
   设置SDK的路径，选择Windows->preferences，在打开的属性框，选择Android，在SDK location中输入你的Android SDK 所在的目录，
   然后按Apply按钮，即可看到安装的SDK包。
   
## 2.4  ADT安装
###   2.4.1 自动安装
   启动Eclipse，选择菜单Help->Install New Software  -->选择选项卡的 Avaible Software，点击右侧按钮“Add”，
   输入https://dl-ssl.google.com/android/eclipse/,如果不支持https，可以选择http://dl-ssl.google.com/android/eclipse/
   选择所有安装包，然后Next安装向导进行下载并安装，安装完成之后，重启Eclipse。
###   2.4.2 手动安装
   也可以使用下载的方式安装，在网络条件不允许的情况下，可以考本其他人的ADT安装。
   下载网站：http://dl.google.com/android/ADT-0.9.7.zip（最新网址参考http://androidappdocs.appspot.com/sdk/eclipse-adt.html）
# 3.测试Android程序的运行
以最经典的例子Hello World作为测试。                                                                                                 