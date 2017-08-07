---
layout: post
title: 在Windows下使用virtualenv
categories: Python
description: 在Windows下使用virtualenv,Multiple Python Versions on Windows
keywords: virtualenv,Multiple Python Versions on Windows
---

在Windows下使用virtualenv，又名：Multiple Python Versions on Windows。本文简要介绍Windows下利用virtualenv创建虚拟环境，实现Python2，Python3两个版本共存。本文假定已安装Python2和Python3。我本机以Python3为主版本，配置了Python3的环境变量。
# 安装virtualenv
首先在系统中安装virtualenv:

``` pip install virtualenv ```
# 创建虚拟环境
* 分别为Python2和Python3虚拟环境创建目录（py2,py3）：

  ``` mkdir py2 ```

  ``` mkdir py3 ```

  ![创建目录](https://github.com/JeetChan/jeetchan.github.io/blob/master/images/posts/python/2017-08-07-mkdir.png)
* 创建Python2虚拟环境

  进入py2目录，运行如下语句：

  ``` virtualenv --python D:\Program\Python2\python.exe ENV ```

  ![py2ENV](https://github.com/JeetChan/jeetchan.github.io/blob/master/images/posts/python/2017-08-07-py2ENV.png)
* 创建Python3虚拟环境

   因为我已设置Python3的环境变量，所以在这里不需要指定Python版本，进入py3目录，运行如下语句：

  ``` virtualenv ENV ```

  ![py3ENV](https://github.com/JeetChan/jeetchan.github.io/blob/master/images/posts/python/2017-08-07-py3ENV.png)
# 激活virtualenv

  在windows中,虚拟环境的激活使用命令：your_env_dir\Scripts\activate，``` activate ```

  ![py2activate](https://github.com/JeetChan/jeetchan.github.io/blob/master/images/posts/python/2017-08-07-py2activate.png)

  ![py3activate](https://github.com/JeetChan/jeetchan.github.io/blob/master/images/posts/python/2017-08-07-py3activate.png)

# 关闭virtualenv
使用下面命令:

``` deactivate ```

![deactivate](https://github.com/JeetChan/jeetchan.github.io/blob/master/images/posts/python/2017-08-07-deactivate.png)
# 参考
[Virtualenv官方文档](https://virtualenv.pypa.io/en/stable/)
# CHANGELOG
* 170807 创建
