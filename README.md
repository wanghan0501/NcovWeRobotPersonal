# 疫情信息自动推送微信机器人

### 简介

使用个人微信账户，利用爬虫信息从网络上搜集疫情信息，用户通过微信消息进行订阅，若出现相关信息，则主动对用户推送信息。

## 功能列表

### 1.爬虫模块

- 1.定时从腾讯新闻获取全国疫情数据（URL: https://news.qq.com/zt2020/page/feiyan.htm）
- 2.按城市/省份对数据进行存储并对比数据是否更新
- 3.推送更新的数据到微信机器人

### 2.微信机器人模块

- 0.微信的正常功能（接收和回复消息、添加好友）
- 1.接收用户订阅，包括省份/城市/关键词
- 2.接收更新的数据并转发给订阅的用户
- 3.取消订阅
- 4.消息数量限制

## 运行环境

- 数据库：Redis
- 部署：Docker