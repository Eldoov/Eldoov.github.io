---
title: "移除Mac Sonoma的大写标识"
date: 2023-11-09
draft: false
---

更新了mac电脑系统，发现只要是开大写键，就一定会出现一个indicator，在多语系统下打字相当烦人。真不知道是苹果哪个设计师拍脑袋想出来的多此一举的功能。

Like this:

![img](/images/sonoma-caps.png)

使用以下指令可以使其消失不见：

```
sudo mkdir -p /Library/Preferences/FeatureFlags/Domain
sudo defaults write /Library/Preferences/FeatureFlags/Domain/UIKit.plist redesigned_text_cursor -dict-add Enabled -bool NO
```