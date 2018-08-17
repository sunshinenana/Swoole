---
title:PHP源码包安装
date: 2018-08-17
updated: 2018-08-17
toc: true
---

## PHP源码安装步骤
官网地址: http://php.net/
- **软件**
    从官网下载最新源码包
- **安装步骤**
    + 1.tar -xjvf php-7.2.8.tar.bz2    (我下载的是php-7.2.8版本)
    + 2.cd php-7.2.8 
    + 3../configure --prefix=/Users/Sara/work/study/soft/php  (php安装目录,自定义)
    + 4.make && make install
- **测试**
    创建一个test.php文件
    执行 /Users/Sara/work/study/soft/php/bin/php test.php
    测试通过,说明php已经安装成功
- **环境变量**
    直接输入php路径执行php文件非常不友好,但是也是为了与自己PHP7.0的环境分开,于是我们要修改环境变量带来更好的体验
    + 设置别名: alias php78="/Users/Sara/work/study/soft/php/bin/php"
    + 重启环境变量: source ~/.bash_profile
    + 测试: php78 test.php
    + 测试通过,说明此php版本设置环境变量成功