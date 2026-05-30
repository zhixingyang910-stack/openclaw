---
使用
read_when:
  -控制+换挡+m
切换
---

#简介：OpenClaw是一个多通道的人工智能代理网关，可以在任何操作系统上运行突耳

query为空p align="center">
突耳
向新人介绍开爪你在你的前面
OpenClaw 🦞
图标“媒体支持”链接]
卡片[卡片发送和接收图像、音频和文档。]
B->G[标题]
B->G[“Web控件UI”]
图标
[Web控件 UI]
图标标题
链接
聊天、配置、会话和节点的浏览器仪表板。图标标题
卡片

“去角质！去角质！”

“多通道网关”
卡片
图标[将 iOS“开始”]>
卡片列链接列链接]>>

标题
卡片
本地默认：
步
[安装 OpenClaw标题]
全局安装最新版的 openclaw：`全局安装最新版的 openclaw：`npm install -g openclaw@latest``
卡片
更新索引
开源的
安装 OpenClaw
卡片

卡片

标题

**“跑步上船”**P

**有什么不同？**

- **Self-hosted**：在硬件和规则上运行
- **Multi-channel**：一个网关同时提供内置通道和捆绑或外部通道插件
- **Agent-native**列
：为具有工具使用，我站在你的前面，OpenClaw*</p align=

**OpenClaw是**自托管网关`22.19+`将你最喜欢的聊天应用程序和频道表面--自力更生，Google Chat，Matrix，Microsoft Teams，Signal，Slack，Telegram，WhatsApp，Zalo-----------------------------------------------------------------------------------------------------------------------------------------------------------

它是如何运作的

```美人鱼
流程图如下所示：
A[聊天应用程序+you']->B[[聊天应用程序]]
B --> C["OpenClaw agent"]
B --> D["CLI"]
B->E[[Web控件 UI]]
  B --> F["macOS app"]
  B --> G["iOS and Android nodes"]
```

The Gateway is the single source of truth for sessions, routing, and channel connections.

## Key capabilities

<Columns>
  <Card title="Multi-channel gateway" icon="network" href="/channels">
    Discord, iMessage, Signal, Slack, Telegram, WhatsApp, WebChat, and more with a single Gateway process.
  </Card>
  <Card title="Plugin channels" icon="plug" href="/tools/plugin">
    Bundled plugins add Matrix, Nostr, Twitch, Zalo, and more in normal current releases.
  </Card>
  <Card title="Multi-agent routing" icon="route" href="/concepts/multi-agent">
    Isolated sessions per agent, workspace, or sender.
  </Card>
  <Card title="Media support" icon="image" href="/nodes/images">
    Send and receive images, audio, and documents.
  </Card>
  <Card title="Web Control UI" icon="monitor" href="/web/control-ui">
    Browser dashboard for chat, config, sessions, and nodes.
  </Card>
  <Card title="Mobile nodes" icon="smartphone" href="/nodes">
    Pair iOS and Android nodes for Canvas, camera, and voice-enabled workflows.
  </Card>
</Columns>

## Quick start

<Steps>
  <Step title="Install OpenClaw">
    ```bash
    npm install -g openclaw@latest
    ```
  </Step>
  <Step title="Onboard and install the service">
    ```bash
    openclaw onboard --install-daemon
    ```
  </Step>
  <Step title="Chat">
    Open the Control UI in your browser and send a message:

    ```bash
    openclaw dashboard
    ```

    Or connect a channel ([Telegram](/channels/telegram) is fastest) and chat from your phone.

  </Step>
</Steps>

Need the full install and dev setup? See [Getting Started](/start/getting-started).

## Dashboard

Open the browser Control UI after the Gateway starts.

- Local default: [http://127.0.0.1:18789/](http://127.0.0.1:18789/)
-OpenClaw是[自托管网关](/web)将你最喜欢的聊天应用程序和频道表面-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------[它是如何运作的](/gateway/tailscale)

<美人鱼流程图如下所示：="center">
  <A[聊天应用程序+you]->B[[你想知道吗]B --> C["OpenClaw agent"]="/whatsapp-openclaw.jpg" B --> D["CLI"]="OpenClaw" B->E[[Web控件 UI]]="420" />
</p>

## Configuration (optional)

Config lives at `~/.openclaw/openclaw.json`.

- If you **do nothing**, OpenClaw uses the bundled OpenClaw agent runtime with per-sender sessions.
- If you want to lock it down, start with `channels.whatsapp.allowFrom` and (for groups) mention rules.

Example:

```json5
{
  channels: {
    whatsapp: {
      allowFrom: ["+15555550123"],
      groups: { "*": { requireMention: true } },
    },
  },
  messages: { groupChat: { mentionPatterns: ["@openclaw"] } },
}
```

## Start here

<Columns>
  <Card title="Docs hubs" href="/start/hubs" icon="book-open">
    All docs and guides, organized by use case.
  </Card>
  <Card title="Configuration" href="/gateway/configuration" icon="settings">
    Core Gateway settings, tokens, and provider config.
  </Card>
  <Card title="Remote access" href="/gateway/remote" icon="globe">
    SSH and tailnet access patterns.
  </Card>
  <Card title="Channels" href="/channels/telegram" icon="message-square">
    Channel-specific setup for Feishu, Microsoft Teams, WhatsApp, Telegram, Discord, and more.
  </Card>
  <Card title="Nodes" href="/nodes" icon="smartphone">
    iOS and Android nodes with pairing, Canvas, camera, and device actions.
  </Card>
  <Card title="Help" href="/help" icon="life-buoy">
    Common fixes and troubleshooting entry point.
  </Card>
</Columns>

## Learn more

<Columns>
  <Card title="Full feature list" href="/concepts/features" icon="list">
    Complete channel, routing, and media capabilities.
  </Card>
  <Card title="Multi-agent routing" href="/concepts/multi-agent" icon="route">
    Workspace isolation and per-agent sessions.
  </Card>
  <Card title="Security" href="/gateway/security" icon="shield">
    Tokens, allowlists, and safety controls.
  </Card>
  <Card title="Troubleshooting" href="/gateway/troubleshooting" icon="wrench">
    Gateway diagnostics and common errors.
  </Card>
  <Card title="About and credits" href="/reference/credits" icon="info">
    Project origins, contributors, and license.
  </Card>
</Columns>
