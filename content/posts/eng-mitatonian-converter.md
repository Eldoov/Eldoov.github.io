---
title: "English to Mitatonian Converter"
date: 2023-04-12
draft: false
---

花了几个小时把英语和自制语言Mitatonian的翻译器写完了。Mitatonian是我自创的一门基于英文音标的语言，使用英文的IPA（国际音标）做字母。由于字母是重新设计过的，自然不会包含在UTF-8，因此如果想要在电脑上显示该语言，需要录入自建的字体“Mitatonian-Regular.tff”。可惜英文键盘并不是基于IPA来设计，Mitatonian的字母全部一共有48个，如果只是录入字体的话，和键盘上的26个字母对应不过来，录入了也等于没录入=。=

这几天试图建立一个字典，无奈手动转换太重复劳动且容易出错，干脆拿python写了个converter一劳永逸。原理是把输入的英文转换成IPA，再经由IPA转换成自制tff字体。问题在于字体和IPA并不是一一对应的，导致直接转换会有很多乱码，拿dictionary做了一个简易版IPAtoFont的翻译器，算是解决问题。最后再调用该翻译器，通过PIL画图输出翻译后的图像。

目前来说有两个功能：

**（1）直接输入英文句子，程序自动输出翻译后的图像。**

输入：

![img](/images/img001.png)

输出：

![img](/images/img02.png)



**（2）文本量大的话，可以直接输入文档txt：**

![img](/images/image-6-1024x260.png)

译文会输出为txt，将字体改为Mitatonian-Regular就可以看到最终效果：

![img](/images/image-4-1024x566.png)



[Github链接](https://github.com/Eldoov/eng-to-mitatonian-converter)
