<div align="center">

# Q

**把繁琐交给脚本，把判断留给自己。**

<sub>MoviePilot 插件开发者 ｜ 自建自用</sub>

<br>

[![MoviePilot](https://img.shields.io/badge/MoviePilot-V2%20%2F%20V3-1f6feb?style=for-the-badge&labelColor=0d1117&logo=github&logoColor=white)](https://github.com/q10710/MoviePilot-Plugins)
[![Plugins](https://img.shields.io/badge/插件-10%20个-3fb950?style=for-the-badge&labelColor=0d1117)](https://github.com/q10710/MoviePilot-Plugins)
[![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?style=for-the-badge&labelColor=0d1117&logo=python&logoColor=white)](https://www.python.org/)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&labelColor=0d1117&logo=docker&logoColor=white)](https://www.docker.com/)

</div>

---

## 关于

自己写、自己改、自己用。用得顺手的东西，就整理出来分享。

插件以 **安全第一** 为前提设计 —— 涉及删除文件、删除订阅、改动下载器的能力，开关默认关闭，或只报告不执行。

<br>

## 插件仓库

<div align="center">

**[q10710 / MoviePilot-Plugins](https://github.com/q10710/MoviePilot-Plugins)**

[![Stars](https://img.shields.io/github/stars/q10710/MoviePilot-Plugins?style=flat-square&labelColor=0d1117&color=8b949e)](https://github.com/q10710/MoviePilot-Plugins/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/q10710/MoviePilot-Plugins?style=flat-square&labelColor=0d1117&color=8b949e)](https://github.com/q10710/MoviePilot-Plugins/commits/main)

</div>

| ｜ | 插件 | 说明 |
| :--: | :--- | :--- |
| 📡 | **订阅助手Q自用版** | 订阅全生命周期管理。H&R 种子下载超时不直接删种，改为移入收容目录保种，按站点 H&R 时长到期后再清理 |
| 🧲 | **H&R助手Q自用版** | H&R 种子标签与做种时长跟踪，支持多下载器，可识别种子在下载器之间的转移做种 |
| 🌊 | **站点流量管理Q自用版** | 按站点分享率自动管理刷流任务：低于下限按最终配置新建并启动，高于上限只暂停不删除 |
| ⚡ | **自动限速Q自用版** | 按标签或全局给 qb / tr 的下载任务限速 |
| 🛡️ | **做种守卫Q自用版** | 检测无效做种与孤儿源文件，连续达标后按策略处置；下载器不可用时整轮跳过，绝不误判 |
| 🔗 | **硬链接检查Q自用版** | 清理「曾经被硬链接、如今链接断开」的残留文件，并清理媒体库里只剩元数据的空壳目录 |
| 🎬 | **洗版守护Q自用版** | 未完结却被误标洗版的订阅自动取消洗版；媒体库文件丢失时自动重置订阅重新下载 |
| 🧹 | **过期订阅清理Q自用版** | 订阅超过设定天数未下载到新剧集时自动取消 |
| 🗑️ | **删档订阅清理Q自用版** | 媒体库条目被删除而订阅仍在、长期不下载时，按配置清理该订阅 |
| 👤 | **渠道用户自动建号Q自用版** | 其他渠道账号首次发消息时，自动按渠道 userid 创建 MoviePilot 普通用户并完成绑定，使其能正常使用查询、搜索、订阅 |

<br>

## 安装

在 MoviePilot 的 `PLUGIN_MARKET` 中加入本仓库：

```text
https://github.com/q10710/MoviePilot-Plugins
```

刷新插件市场，搜索插件名安装即可。建议配置 `GITHUB_TOKEN`，避免触发 API 限流。

<br>

## 设计原则

> **数据安全优先** — 删除类能力默认关闭，媒体库侧默认只报告不删除。
>
> **口径写清楚** — 每个插件的判据、边界与上游来源，都记录在仓库 README 和更新说明里。
>
> **改动可回滚** — 先自测、再小步发布，保留完整历史版本说明。

<br>

---

<div align="center">

<sub>基于上游项目的改造版，版权归原作者所有 · 遵循上游许可协议</sub>

</div>
