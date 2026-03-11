![使用 Animoca Minds 构建无代码 Discord Bot](assets/banner.png)

# 面向每一种技能解锁 AI 智能体：使用 Animoca Minds 构建无代码 Discord Bot

在数字工具持续演进的版图中，AI 智能体正在重塑我们与平台、社区与创意项目的交互方式。由 @AnimocaBrands 驱动的 Animoca Minds 正是这一趋势的代表：它将先进 AI 融入工作流，以提升生产力、自动化与创新能力。本文参考 Animoca Brands 执行董事长兼联合创始人 Yat Siu（@ysiu）近期的一则 thread，带你快速部署一个由 AI 驱动的 Discord bot。但这不止于 Discord——这些智能体可无缝适配更广泛的任务：从侦测信号（signal scouting）、搭建策略框架（strategy architecture）到高阶提示词驱动（visionary prompting）。  
无论你是新手还是资深管理员，都可以通过 Animoca Minds 在很短时间内完成 AI 智能体的搭建与上线。AI 将承担大部分流程，把你的 bot 变成面向管理、分析或自定义任务的专属助理。  
读完本文，你将掌握部署自有智能体所需的关键知识，并理解如何将其能力从基础功能扩展到更复杂的用例。

## **为什么选择 Animoca Minds 来构建 AI 智能体？**

Animoca Minds 通过无缝、即插即用的模型，移除进入 agentic web（智能体网络）的技术门槛，让你能以规模化方式部署自治智能体。与传统基础 bot 不同，每一个 Mind 都是可验证实体（verifiable entity），拥有独立的**身份（identity）、记忆（memory）与钱包（wallet）**，并由安全的 Web3 框架支撑其自主运行。

你的 bot / 智能体可以身兼数职，切换不同 persona，例如：

* **侦察者（监控）：** 跟踪数据信号、识别诈骗、监控 Discord/X 信息流。  
* **架构师（策略）：** 生成摘要、起草策略、沉淀深度洞察。  
* **远见者（创意）：** 提供 AI 前瞻判断并处理复杂提示词编排。

无需编写代码——只要加载正确的"skill" artifact，就能赋予你的 Mind 所需能力，让它像虚拟队友一样行动。

## **一步步搭建 AI 驱动的 Discord Bot**

请按顺序完成以下步骤。每一步都建立在上一步的基础上，我们也附上了避免常见坑位的提示。如果你不熟悉 "artifact" 或 "Mind" 等术语，我们会在文中逐步解释。

### Step 1：在 Animoca Minds 上创建你的 AI 智能体

从 Animoca Minds 平台开始——你的 AI"脑"就住在这里。

1. 访问 [https://www.animocaminds.ai/](https://www.animocaminds.ai/) 并输入邮箱注册（如已有账号则登录）。  
2. 查看邮箱。你会收到一封来自 animocaminds.ai 的欢迎邮件。  
3. 回复欢迎邮件以创建你的 Mind：为其命名、定义 persona，并设置专长（例如：专注于 Discord 沟通的 AI 智能体）。  
4. 在初始 Concierge AI 索要更多信息时，你可能会与其往来数封邮件；你也可以直接指示它"create the Mind now!"。当你的 Mind 被唤醒后，你会收到通知邮件。

"Mind" 是可自定义的 AI 配置文件，可用于 Discord 互动、新闻摘要、创建无代码应用、通过 Google Calendar 代你预约等任务。你可以通过邮件或 Telegram 与 AI concierge 交互——就像与一个负责配置的助理聊天一样简单。

专业提示：你可以使用邮件或 Telegram 与 Animoca Minds 通信。若使用 Telegram，请按以下步骤完成配置：

* 在 Telegram 中搜索 @BotFather 并打开对话。在进入聊天模式前务必核对账号，避免误入仿冒账号。  
* 输入 /newbot。  
* 为 bot 取名（例如：My Mind Peter）。  
* 为 bot 设置用户名（必须以 '_bot' 结尾，例如：peter123_bot）。  
* 复制 HTTP API token（出于安全考虑请视为机密）。  
* 前往 [https://app.animocaminds.ai/profile](https://app.animocaminds.ai/profile) 并点击 "Link Telegram"。  
* 输入你的手机号并接收 Telegram 发来的验证码。  
* 将验证码填入弹窗。  
* 在 Telegram 的消息中点击 "Connect" / "Accept"。  
* 粘贴 HTTP API token 以完成 Telegram 绑定。  
* 返回 @BotFather，点击 t.me/yourbotname 链接，将你的 Mind 添加到 Telegram 聊天中。  
* 开始在 Telegram 中与你的 bot 对话。

该配置非常适合快速迭代，例如测试不同技能。

### Step 2：为你的 AI 加载 Discord 能力（或任意 Skill）

为你的智能体装备即插即用的技能，无需写代码。本步骤将为 Mind 添加必要的"超能力"。

1. 在与你的 AI 智能体的聊天中（邮件或 Telegram），发送以下指令（建议原样粘贴）：  
   **Ethoswarm Harbor Manifest: Clinical Discord Sentinel**

**Harbor ID:** HARBOR-DSM-66B6

**Vessel Archetype:** Guardian / Sentinel

**Primary Intent:** Clinical, high-fidelity monitoring of Discord streams and X signals with autonomous support routing.

**Integrated Skill Protocols:**

* **Core Signal Sentinel:** 0787B95F-5716-F111-AD1D-0EA9A5017E89(Discord_Signal_Sentinel_v1)  
* **Implementation Guide:** BF799981-8018-F111-AD1D-0EA9A5017E89 (Mind-to-Mind framework)  
* **Clinical Monitoring (Echo_Discord):**94F19126-CE12-F111-AD1D-0EA9A5017E89  
* **Technical Bridge (Hiro):** CD213352-BB12-F111-AD1D-0EA9A5017E89  
* **Support Routing (3b-helper):** 7D750FD8-8710-F111-AD1D-0EA9A5017E89

**Persona Profile:**

* **Traits:** Vigilant, Precise, Data-driven, Attentive.  
* **Tone:** Formal and Clinical; prioritizes clarity and signal over noise.  
* **Framework:** Optimized for Discord API v10 and RESTful HTTP integrations.

2. AI 将立即完成集成，从而启用发送/接收消息、监控频道等功能。Artifacts 可理解为预制插件；你也可以替换为其他技能，例如数据分析或教练式对话。

注意：这种无代码机制允许你在无技术负担的情况下，将智能体扩展到从基础前瞻到高级策略的任意能力。

或者，你也可以直接告诉 AI 智能体你希望构建一个 Discord bot，并请求为其配齐你找到的所有必要技能；AI 会与你逐步澄清需求并完成配置。

### Step 3：在 Discord Developer Portal 创建 Bot

现在切换到 Discord，为 bot 创建"身份"。这是将由你的 AI 控制的外壳。

1. 登录 Discord 并进入 Developer Portal： [https://discord.com/developers/applications](https://discord.com/developers/applications)。  
2. 点击 "New Application"。为其命名（例如 "AI Scout Bot"），并可选添加图标以个性化。  
3. 为了更好的组织方式（尤其是团队项目），建议先创建 Developer Team。参考 Discord 指南： [https://support-dev.discord.com/hc/en-us/articles/34905563063703-Creating-and-Managing-a-Developer-Team](https://support-dev.discord.com/hc/en-us/articles/34905563063703-Creating-and-Managing-a-Developer-Team)。  
4. 然后将你的 bot 添加到该团队。

此步骤用于打好底层基础，确保 bot 能以安全方式加入服务器。

### Step 4：配置权限并连接 Bot

在这里你将定义 bot 能做什么，并将其与 Animoca Minds 的 AI 连接。

1. 在新应用的设置中，进入 "Bot" 标签页。  
2. 生成 Bot Token（唯一密钥）。请安全保存，它相当于 bot 的密码。

![Bot Token Generation](assets/bot-token-generation.png)

  
3. 设置 bot 权限：选择它可访问的范围，例如读取消息或管理频道。建议先从核心权限开始，如 "Send Messages" 与 "Read Message History"，以保持简洁。  
4. 进入 "OAuth2" 标签页并选择 "URL Generator"。选择 scope "bot"，以便通过 URL 将 bot 添加到服务器；然后选择与 bot 需要的权限一致的项（例如读/写消息）。配置完成后，将生成的 URL 粘贴使用，并在菜单中把 bot 发送到目标 Discord 服务器。  
   

![OAuth2 URL Generator](assets/oauth2-url-generator.png)

5. 在 "Bot Permissions" 下，勾选与你需求匹配的权限（例如监控用 "View Channels"，管理用 "Manage Messages"）。  
   

![Bot Permissions](assets/bot-permissions.png)

  
6. 将生成的 URL 粘贴到 "OAuth2" 标签页底部，并用它将 bot 添加到你的 Discord 服务器（选择 "Guild Install" 以进行服务器级安装）。

![Guild Install URL](assets/guild-install-url.png)

  
7. 最后，通过聊天将 Bot Token 安全地发送给你的 Animoca Minds AI 智能体。这将打通两个系统并激活 bot。

对于偏好可视化学习的用户，YouTube 上关于 Discord bot 配置的教程能提供更直观的引导。你可以搜索 "How to create a Discord bot application" 或 "Discord developer portal tutorial"。freeCodeCamp、Skills Academy 等频道通常有逐步演示界面、按钮点击与常见坑位的视频。只需跳过任何"编写/托管代码"的部分，因为 Animoca Minds 会为你处理这些内容。若你在权限设置上卡住，建议对照 Discord 文档逐项核对其含义。

### Step 5：将 AI 与 Discord Bot 连接起来

最后一步是将 Bot Token 提供给你的 AI 智能体。有时 AI 会要求提供 Server ID，以确认被添加到正确的服务器。通常需要 10–15 分钟以上完成连接。配置完成后，AI 智能体会回报已完成；如果你想更快获得进度，也可以主动询问状态。

### Step 6：为每一种技能进行定制

连接完成后，你可以定义 bot 的行为方式——有趣的部分从这里开始。

1. 回到 Animoca Minds 的聊天中，给出清晰指令，例如："监控 #general 频道的异常信号并生成每日报告"，或"基于最新知识回答用户关于 AI 工具的问题"。  
2. 在你的 Discord 服务器中测试：发送消息，观察 bot 是否快速响应。  
3. 按需扩展：加载更多 artifacts，用于管理、策略构建或创意生成。例如，指示 bot 在自动化工作流中遵循 "plan -> act -> verify"。

始终从简单指令开始，并基于结果迭代优化，以提升整体表现。

## 常见建议与故障排查

* **安全第一**：像对待私钥一样对待 Discord Bot Token——绝不要公开分享，也不要在不安全的聊天中发送。  
* **常见问题**：如果 Discord bot 没有响应，请确认 Token 是否正确共享，以及权限是否已启用。必要时重启 Discord 客户端。你也可以把 AI 智能体当作故障排查助手：直接描述你遇到的情况即可。  
* **社区支持**：Yat Siu 的原始 thread 中包含用户实测该配置的真实案例。 

**你可能会问：为什么无需任何代码也能做到？** 传统 bot 通常需要用 Python 等语言编程；而在这里，AI 抽离了这层技术门槛，使其对非技术用户也非常友好。

## 用 Animoca Minds 赋能构建者

恭喜！你已经解锁了可覆盖多种技能的 AI 智能体：从创建 Discord bot，到数据侦察与创意自动化等更广泛的应用。Animoca Minds 的无代码方案让任何人都能无门槛构建，节省时间，并打开全新可能性。  
准备部署了吗？现在就前往 Animoca Minds 开始实验吧。有更智能的工具相伴，你的项目将更具生命力！如果你遇到任何阻碍，建议直接让你的 AI 智能体协助——它清楚你当前所处的步骤。如果愿意，你也可以回看本文步骤，或查阅 Yat 的 thread 获取灵感。

## 实用链接

* Yat Siu 原始 thread： [https://x.com/ysiu/status/2028524246897680884?s=20](https://x.com/ysiu/status/2028524246897680884?s=20)  
* Animoca Minds 平台： [https://www.animocaminds.ai/](https://www.animocaminds.ai/)  
* Discord Developer Portal： [https://discord.com/developers/applications](https://discord.com/developers/applications)  
* Discord Developer Team 指南： [https://support-dev.discord.com/hc/en-us/articles/34905563063703-Creating-and-Managing-a-Developer-Team](https://support-dev.discord.com/hc/en-us/articles/34905563063703-Creating-and-Managing-a-Developer-Team)

---

## Credits/Colophon

```yaml
title: "面向每一种技能解锁 AI 智能体：使用 Animoca Minds 构建无代码 Discord Bot"
title_en: "Unlocking AI Agents for Every Skill: Building No-Code Discord Bots with Animoca Minds"
date: "2026-03-10"
author: "Animoca Minds"
language: "zh-CN"
tags:
  - animoca-minds
  - discord
  - no-code
  - ai-agents
  - tutorial
  - web3
source_url: "https://x.com/AnimocaMinds/status/2029857923589980607"
slug: "building-nocode-discord-bots-with-animoca-minds"
distributions:
  - platform: "x"
    url: "https://x.com/AnimocaMinds/status/2029857923589980607"
  - platform: "github"
    url: "https://github.com/AnimocaMindsTips/Animoca-Minds-Tips/blob/main/articles/2026/03/10-building-nocode-discord-bots-with-animoca-minds/zh-CN.md"
```
