![使用Animoca Minds搭建Steam新闻监控Discord机器人指南](assets/banner.png)

# 使用Animoca Minds搭建Steam新闻监控Discord机器人指南

让游戏社区实时了解Steam新闻，不再需要手动操作或编程技能。本指南将带您完成使用[Animoca Minds](https://www.animocaminds.ai/)配置无代码自动化系统的步骤，该系统可监控[Steam](https://store.steampowered.com/)的RSS订阅源，并自动将每日新闻摘要发送到Discord频道或您的邮件收件箱。

该系统连接三个主要组件：Steam的RSS订阅源、Animoca Minds AI平台和您首选的通知渠道。无需编程，AI代理将代您处理监控、摘要和发布工作。

## 为什么使用Animoca Minds监控Steam新闻？

Animoca Minds将RSS订阅源解析和定时发布等复杂任务转化为简单的自然语言指令，简化了AI驱动的自动化流程。对于游戏社区来说，及时获取有关新游发布、促销活动或补丁的更新，可以在不需要开发资源的情况下显著提升用户参与度。

您的自动化代理可以：

- 扫描[Steam的RSS订阅源](https://store.steampowered.com/feeds/news.xml)获取新文章或公告
- 生成按类型或关键词筛选的简洁每日摘要
- 自动向Discord频道发布更新或通过邮件发送
- 通过简单的后续指令适应不断变化的偏好

## 前提条件

开始前，请确保您拥有：

- 具有管理员或机器人管理权限的Discord服务器（Discord推送选项所需）
- [Animoca Minds](https://www.animocaminds.ai/)账户

## 第一步：创建和配置Discord机器人

如果您希望将更新发布到Discord频道，请执行此步骤。如果您更喜欢邮件推送，请直接跳到第二步。

### 1.1 创建应用程序

1. 前往[Discord Developer Portal](https://discord.com/developers/applications)。
2. 点击**New Application**。
3. 输入机器人名称（例如："Steam News Monitor"），然后点击**Create**。

### 1.2 获取机器人令牌

1. 在左侧边栏中，导航到**Bot**选项卡。
2. 点击**Add Bot**（如果机器人已存在，则点击**Reset Token**）。
3. 复制令牌并安全保存——配置Animoca Mind时需要用到。

### 1.3 设置机器人权限

1. 前往**OAuth2 → URL Generator**。
2. 在Scopes下，选择**bot**。
3. 启用以下权限：**Send Messages**、**Embed Links**和**Read Message History**。
4. 复制生成的邀请URL，将机器人添加到您的服务器。

> **安全提示：** 只授予机器人所需的最低权限以降低风险。详情请参阅[Discord机器人权限指南](https://support-dev.discord.com/hc/en-us/articles/34905563063703)。

## 第二步：设置您的Animoca Mind

1. 访问[animocaminds.ai](https://www.animocaminds.ai/)并登录或创建账户。
2. 检查收件箱中来自Animoca Minds的欢迎邮件（最多等待5分钟）。
3. 回复邮件开始设置新的Mind。定义：
   - **名称：** 例如"Steam Scout"
   - **角色：** 例如"游戏新闻专家"
   - **专长：** 例如"RSS监控和Discord发布"
4. Concierge AI可能会提问以完善设置。如需加速，回复：*"现在创建Mind。"*
5. Mind准备好后您将收到确认通知。

## 第三步：加载Steam技能并给出指令

1. 在与AI代理的对话中，指示其加载Steam技能：
   > *"加载工件 Steam_Web_API_v1"*

   您可以在Animoca Minds中找到它。如果工件ID已更改，请询问：*"列出可用的Steam工件。"*

2. 如果使用Discord，将您的**Discord机器人令牌**作为安全凭证与Mind共享。

3. 提供初始指令。示例：
   - *"每天给我推送Steam上动作、动作RPG和RPG游戏的新闻。"*
   - *"告诉我香港地区的Steam服务状态。"*
   - *"每天早上9点在我的Discord频道发布Steam每日新闻摘要。"*

## 第四步：测试和自定义

1. 向您的Mind发送测试指令：
   - Discord：*"生成一个Steam新闻摘要样本并发布到我的Discord频道。"*
   - 邮件：*"生成一个Steam新闻摘要样本并通过邮件发送给我。"*
2. 检查您的Discord频道或收件箱中的更新。
3. 添加筛选条件进行细化——例如：*"仅包含标记为'魂系'或'开放世界'游戏的新闻。"*
4. Mind在各会话间保留指令，因此更新是累积的。

## 有用链接

- [Animoca Minds](https://www.animocaminds.ai/)
- [Discord Developer Portal](https://discord.com/developers/applications)
- [Steam商店](https://store.steampowered.com/)
- [Steam新闻RSS订阅源](https://store.steampowered.com/feeds/news.xml)
- [Discord机器人权限指南](https://support-dev.discord.com/hc/en-us/articles/34905563063703)

---
title: "使用Animoca Minds搭建Steam新闻监控Discord机器人指南"
title_en: "Guide to Setting Up a Steam News Monitoring Discord Bot with Animoca Minds"
date: "2026-03-15"
author: "Animoca Minds"
language: "zh-CN"
content_type: "article"
source_platform: "x"
source_url: "https://x.com/AnimocaMinds/status/2032407420073623613"
slug: "setting-up-steam-news-monitoring-animoca-minds"
distributions:
  - platform: "x"
    url: "https://x.com/AnimocaMinds/status/2032407420073623613"
  - platform: "github"
    url: "https://github.com/AnimocaMinds/Animoca-Minds-Tips/blob/main/posts/2026/03/15-setting-up-steam-news-monitoring-animoca-minds/zh-CN.md"
tags:
  - animoca-minds
  - steam
  - gaming
  - discord-bot
  - rss-monitoring
  - automation
  - no-code
---