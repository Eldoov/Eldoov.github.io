---
title: "Sec+ 社会工程学名词笔记"
date: 2024-1-18T16:51:50
draft: false
---

#### Sec+ 社会工程学名词笔记

**Pharming 域欺骗**

Pharming的目的是将一个网站的流量重定向至另一个虚假网站，方法有改变受害者计算机上的hosts文件、DNS投毒、或者利用DNS服务器软件的漏洞进行。

![Phishing vs. Pharming - Valimail](https://www.valimail.com/wp-content/uploads/2022/10/article-phishing-vs-pharming_Img1-1024x859-1.png)



**Water hole attacks 水坑攻击**

指攻击者在受信任的网站传播恶意软件，方法有攻击网站浏览器和浏览器插件漏洞，或者服务器活客户端的漏洞。

攻击者一般不会建立自己的网站。这有两个原因。首先，没有人会访问他们的网站。第二，安全专家经常使用一种叫做黑名单的控制手段。黑名单建立了已知的恶意网站列表，然后在网络边界用内容过滤器阻止它们，防止用户意外地感染自己。

![img](https://img-blog.csdnimg.cn/8a2cf24d86c4458aa4fe52ffbebf1659.png?x-oss-process=image/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5qC85rSb57Gz54ix5a2m5Lmg,size_20,color_FFFFFF,t_70,g_se,x_16)

1. 攻击者识别并破坏了一个他们的受众可能会访问的高度目标网站；
2. 接下来，攻击者选择一个客户端漏洞，破坏网站访问者浏览器的安全，然后捆绑一个僵尸网络有效载荷，将受感染的系统加入到攻击者的僵尸网络中；
3. 然后攻击者将该恶意软件放在被破坏的网站上； 
4. 等待受害者上钩。



**Credential Harvesting**

攻击者收集到大量用户的私密信息，目的主要在于贩卖信息而不是使用。



**SPIM**

SPam Instant Messaging（所以说为什么要专门搞一个别的名词……）



**Hoax攻击**

通过邮件、网站弹窗或者社交网络发送欺骗信息，例如“您的电脑已中毒”。



**Kiting** is the act of continually registering, deleting, and reregistering a name within the five-day grace period without having to pay for it.

白嫖域名



**Tasting** is a Domain Name Server (DNS) exploit that involves registering a domain temporarily to see how many hits it generates within the five-day grace period.

测试域名在注册后五天内的点击次数