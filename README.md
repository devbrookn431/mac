# ClashX Pro 停更后：Mac 上的 Clash 客户端怎么换

这页整理 ClashX 系列的仓库现状，以及五个 Mac 客户端的系统要求、内核和配置迁移说明。核对日为 2026-11-14，仓库状态以对应项目仓库为准，版本与日期以各项目发布页当天显示为准。迁移信息以各客户端 README 为准。

---

[![核对](https://img.shields.io/badge/%E6%A0%B8%E5%AF%B9-2026--11--14-7c5cff)](#toc) [![主题](https://img.shields.io/badge/%E4%B8%BB%E9%A2%98-ClashX%20Pro-2f7bea)](#toc) [![形式](https://img.shields.io/badge/%E5%BD%A2%E5%BC%8F-%E6%97%B6%E9%97%B4%E7%BA%BF%20%2B%20%E6%B8%85%E5%8D%95-6f56d9)](#toc) [![出处](https://img.shields.io/badge/%E5%87%BA%E5%A4%84-%E9%A1%B9%E7%9B%AE%E4%BB%93%E5%BA%93%E4%B8%8E%E5%8F%91%E5%B8%83%E9%A1%B5-1fa37a)](#toc)

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="images/banner-dark.svg">
    <img src="images/banner.svg" alt="ClashX Pro 停更后：Mac 上的 Clash 客户端怎么换，时间线、替代客户端与迁移清单" width="100%">
  </picture>
</p>

> [!NOTE]
> 📌 本页只整理停更时间点、替代客户端的出处与对照和迁移步骤，不提供旧版安装包、订阅链接或配置模板。
>
> 🔎 每一行都带出处链接；日期和版本号以各项目仓库、发布页当天显示为准，本页核对日 2026-11-14。
>
> ⚠️ 表里标「待核」的行，是本页没有读到原文的内容，不要当结论用。

> 标签说明：`官方` 取自项目仓库、发布页或归档说明 · `自述` 客户端自己的 README 或说明里的说法 · `待核` 本页没有读到原文，不当结论用

<a id="toc"></a>
## 📋 目录导航

- [🕰 时间线](#shijian) · [💻 替代客户端](#tidai) · [📋 迁移清单](#qianyi) · [🔤 旧名称](#jiuming)

<a id="shijian"></a>
## 停更时间线

*给想先弄清 ClashX 与 ClashX Pro 是什么时候停的人看。*

*相关：[替代客户端对照](#tidai)*

下表记录仓库状态、提交日期和发布日期。ClashX Pro 的停更日期，官方没有说明。

| 日期 | 事项 | 对应项目 | 出处 | 标签 |
| --- | --- | --- | --- | --- |
| 2026-11-14 | 核对日页面返回 404；官方没有说明原因 | Dreamacro/clash | [仓库页面](https://github.com/Dreamacro/clash) | `待⁠核` |
| 2026-11-14 | 核对日页面返回 404；官方没有说明原因 | yichengchen/clashX | [仓库页面](https://github.com/yichengchen/clashX) | `待⁠核` |
| 2026-11-14 | 旧版 README 单列 Pro，称其支持增强模式与原生 Apple Silicon | ClashX Pro | [旧版 README](https://github.com/MetaCubeX/ClashX.Meta/blob/master/README.md) | `自⁠述` |
| 2022-03-24 | 默认分支 master 的最近提交；该分支 README 仍称基于 Dreamacro/clash | ClashX.Meta：master 分支 | [提交记录](https://github.com/MetaCubeX/ClashX.Meta/commits/master)、[分支说明](https://github.com/MetaCubeX/ClashX.Meta/blob/master/README.md) | `官⁠方` |
| 2026-11-13 | meta 分支最近提交与 v1.4.48 发布同日；该分支 README 称基于 Mihomo，仓库未归档 | ClashX.Meta：meta 分支 | [发布记录](https://github.com/MetaCubeX/ClashX.Meta/releases/tag/v1.4.48)、[分支说明](https://github.com/MetaCubeX/ClashX.Meta/blob/meta/README.md) | `官⁠方` |
| 2023-10-31 | 最近发布 v1.3.8；仓库现已归档，README 为 Removed | Clash Verge | [仓库说明](https://github.com/zzzgydi/clash-verge) | `官⁠方` |

**[⬆ 回到目录](#toc)**

<a id="tidai"></a>
## 替代客户端对照

*给要在 Mac 上换客户端、想先看芯片和系统门槛的人看。*

*相关：[停更时间线](#shijian)、[迁移清单](#qianyi)*

系统与内核信息来自各客户端 README，最近发布信息截至核对日。ClashX Meta 的默认分支保留旧 ClashX 说明，下表采用 meta 分支 README。

| 客户端 | 芯片与系统 | 内核与最近发布日 | 出处 | 标签 |
| --- | --- | --- | --- | --- |
| ClashX Meta | 仅写 for Mac；芯片与最低系统版本 README 未写明 | Mihomo Core；v1.4.48，2026-11-13 | [README](https://github.com/MetaCubeX/ClashX.Meta/blob/meta/README.md)、[发布记录](https://github.com/MetaCubeX/ClashX.Meta/releases/tag/v1.4.48) | `自⁠述` |
| Clash Verge Rev | macOS 11+；Intel / Apple | Clash.Meta（mihomo）；可切换 Alpha 内核；v2.5.10，2026-11-03 | [README](https://github.com/clash-verge-rev/clash-verge-rev/blob/dev/README.md)、[发布记录](https://github.com/clash-verge-rev/clash-verge-rev/releases) | `自⁠述` |
| Clash Party | 系统与芯片要求 README 未写明 | Smart 与 Mihomo（Clash Meta）；v2.0.4，2026-10-18 | [README](https://github.com/mihomo-party-org/clash-party/blob/smart_core/README.md)、[发布记录](https://github.com/mihomo-party-org/clash-party/releases) | `自⁠述` |
| FlClash | macOS 12 及以上；Apple Silicon / Intel | mihomo（Clash.Meta）；v0.9.3，2026-11-04 | [README](https://github.com/chen08209/FlClash/blob/main/README.md)、[发布记录](https://github.com/chen08209/FlClash/releases) | `自⁠述` |
| Clash Mi | macOS 12 及以上；Intel / Apple Silicon | Mihomo（Clash.Meta）；v1.0.32.1803，2026-11-03 | [README](https://github.com/KaringX/clashmi/blob/main/README.md)、[发布记录](https://github.com/KaringX/clashmi/releases) | `自⁠述` |

**[⬆ 回到目录](#toc)**

<a id="qianyi"></a>
## 从 ClashX Pro 搬到新客户端的清单

*给已经决定换客户端、想按项目逐项搬的人看。*

*相关：[替代客户端对照](#tidai)、[旧名称与易混写法](#jiuming)*

下表列出 README 明确写出的配置位置、导入方式及管理功能。旧版 ClashX 的目录说明不能用来确认 ClashX Pro 的配置位置。

| 项目 | 怎么搬 | 注意 | 出处 | 标签 |
| --- | --- | --- | --- | --- |
| ClashX 旧版配置 | 默认目录为 `$HOME/.config/clash`，文件名为 `config.yaml`；Config 菜单可切换自定义配置 | 来自 master 分支旧说明；ClashX Pro 的目录，官方没有说明 | [旧版 README](https://github.com/MetaCubeX/ClashX.Meta/blob/master/README.md) | `自⁠述` |
| ClashX Meta | 默认目录为 `$HOME/.config/clash.meta`，文件名为 `config.yaml`；README 列有 URL scheme 导入方式 | 目录与旧版 ClashX 不同；URL scheme 小节标注 May not work | [README](https://github.com/MetaCubeX/ClashX.Meta/blob/meta/README.md) | `自⁠述` |
| FlClash | README 写明可从订阅或文件导入配置 | 列有系统代理、TUN 模式及 WebDAV、本地文件备份恢复 | [README](https://github.com/chen08209/FlClash/blob/main/README.md) | `自⁠述` |
| Clash Verge Rev | 列有配置管理、Merge 和 Script 增强，以及 WebDAV 配置备份同步 | README 未写具体步骤；列有系统代理与 TUN 模式 | [README](https://github.com/clash-verge-rev/clash-verge-rev/blob/dev/README.md) | `自⁠述` |
| Clash Party | 列有 WebDAV 备份恢复与覆写功能 | README 未写具体步骤；列有无需服务模式的 Tun | [README](https://github.com/mihomo-party-org/clash-party/blob/smart_core/README.md) | `自⁠述` |
| Clash Mi | README 写明内核基于 YAML 配置运行，可使用订阅 | README 未写具体步骤；自带 zashboard 面板 | [README](https://github.com/KaringX/clashmi/blob/main/README.md) | `自⁠述` |

**[⬆ 回到目录](#toc)**

<a id="jiuming"></a>
## 旧名称与易混写法

*给读旧资料、分不清 ClashX、ClashX Pro、ClashX Meta 的人看。*

*相关：[停更时间线](#shijian)*

<details>
<summary>展开：旧名称与易混写法对照（附录性质，不含主表）</summary>

- ClashX、ClashX Pro、ClashX Meta：ClashX Meta README 提醒，这些客户端不附带代理服务器，也没有以这些名称设立的官方网站，并警示冒用官方身份的页面。[出处](https://github.com/MetaCubeX/ClashX.Meta/blob/meta/README.md)
- ClashX 与 Clash：旧版 README 将 ClashX 描述为基于 Clash 的 Mac 规则代理客户端。[出处](https://github.com/MetaCubeX/ClashX.Meta/blob/master/README.md)
- ClashX Pro 与 ClashX：旧版 README 为 Pro 单列说明，提到增强模式和原生 Apple Silicon 支持。[出处](https://github.com/MetaCubeX/ClashX.Meta/blob/master/README.md)
- Clash Verge 与 Clash Verge Rev：Rev 的 README 将项目称为 Clash Verge 的延续；原 Clash Verge 仓库已归档。[Rev 说明](https://github.com/clash-verge-rev/clash-verge-rev/blob/dev/README.md)、[原仓库](https://github.com/zzzgydi/clash-verge)
- Mihomo 与 Clash.Meta：旧仓库地址跳转到 Mihomo；客户端 README 中也有将这两个名称并列的写法。[内核仓库](https://github.com/MetaCubeX/mihomo)、[FlClash 说明](https://github.com/chen08209/FlClash/blob/main/README.md)
- Mihomo Party 与 Clash Party：旧仓库地址跳转到 Clash Party，当前 README 使用 Clash Party 名称。[项目说明](https://github.com/mihomo-party-org/clash-party/blob/smart_core/README.md)

</details>

**[⬆ 回到目录](#toc)**
