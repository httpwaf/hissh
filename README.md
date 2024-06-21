# hissh

#### 一 、介绍
hissh是一款开源的SSH命令审计产品。

#### 二 、SSH审计原因
##### 1、黑客通过钓鱼控制了管理员电脑

​    大多渗透攻击都是通过各种钓鱼套路在客服或者技术人员电脑植入后门，从而进一步入侵服务器。

##### 2、未知RCE漏洞，直接入侵了服务器

    现在高级漏洞都不直接公开了，上升为国家之间情报战略，秘密潜伏的比破坏的多得多。


#### 三、系统内核要求和主要功能
​要求内核版本大于4.10，推荐2021年以后的linux发行版本：
    Ubuntu 20.10+
    
    Fedora 31+
    
    RHEL 8.2+
    
    Debian 11+
    

1、 全面审计用户如root的操作命令，对任何终端都不信任，危险指令、删除日志、异常、异地登录等实时报警。

2 、全面防御对SSH服务的扫描探测、密码破解等。

3 、编译方法用root权限直接make运行./hissh命令即可，然后另外开一个终端运行任意命令就会打印如下内容：
TIME     COMM             PID     CMD

07:31:41 bash             193029  ls -al

07:34:00 bash             193797  ip a

07:34:10 bash             193797  ip a



#### 四、商业版演示地址

商业版集成在openhfw里了，演示地址 [http://101.42.31.94:9998/ok.html/](http://101.42.31.94:9998/ok.html)

#### 五、源码部署请加微信号httpwaf

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/wechat.png)

#### 六、来一张首页大图

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/home.png)
