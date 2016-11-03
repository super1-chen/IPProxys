﻿# IPProxys
IPProxys代理池项目，提供代理ip
<br/>
详细使用方式，请看我的博客:
http://www.cnblogs.com/qiyeboy/p/5693128.html
<br/>
linux debian下:
<br/>
需要安装sqlite数据库:
apt-get install sqlite sqlite3
<br/>
安装requests库
pip install requests
<br/>
安装lxml
apt-get install python-lxml
<br/>
我的微信公众号:
<br/>
![](qiye2.jpg)
<br/>
希望大家提供更多的代理网站，现在爬取的好用的代理ip还是太少。

## 如何使用

将项目目录clone到当前文件夹

$ git clone 

切换工程目录

```
$ cd IPProxys
```

运行脚本

```
python IPProxys.py
```

## API 使用方法

#### 模式
```
GET /
```

####参数 


| 参数名 | 类型 | 描述 | 是否必填 |
| ----| ---- | ---- | ---- |
| types | int | 0: 高匿代理, 1 透明  | 是 |
| protocol | int | 0: http, 1 https | 否 |
| count | int | 数量 | 是 |
| country | str | 国家 | 否 |
| area | str | 国家 |否|



#### 例子

```
GET /?types=0&count=10 # 获取10个代理
```

<br/>
-----------------------------2016-10-27----------------------------
<br/>
1.增加对代理的检测，测试是否能真正访问到网址，实现代理
<br/>
2.添加通过正则表达式和加载插件解析网页的方式
<br/>
3.又增加一个新的代理网站
<br/>

-----------------------------2016-7-20----------------------------
<br/>
修复bug ,将数据库进行压缩
<br/>
