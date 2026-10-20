# 一加16提权越狱

**OnePlus 16 / PYB110 专用临时 root 工具 · 当前版本 v2.3.3**

[下载 v2.3.3 APK](https://github.com/xingranya/OnePlus16-Jailbreak/releases/download/v2.3.3/OneKeyJB-v2.3.3.apk) · [版本下载](https://github.com/xingranya/OnePlus16-Jailbreak/releases) · [文件校验](https://github.com/xingranya/OnePlus16-Jailbreak/releases/download/v2.3.3/OneKeyJB-v2.3.3.apk.sha256)

本仓库用于发布安装包和使用说明。软件免费，禁止倒卖；QQ群：**1121682811**。赞赏自愿，不影响任何功能。

## 适用范围

| 项目 | 要求 |
|---|---|
| 设备 | 一加 16 / OnePlus 16，型号 `PYB110` |
| 系统 | ColorOS 17 / Android 17 |
| 内核 | `6.18.21-android17-5-gf957accaf563-ab15926176-4k` |
| 权限服务 | [Stellar](https://github.com/roro2239/Stellar/releases)，启动后授权本应用 |
| 管理器 | [KernelSU-Next v3.4.2](https://github.com/KernelSU-Next/KernelSU-Next/releases/tag/v3.4.2)，或实验性的 [SukiSU Ultra v4.2.1](https://github.com/SukiSU-Ultra/SukiSU-Ultra/releases/tag/v4.2.1) |

只支持表中机型和精确内核版本。机型或内核不匹配时请停止操作。

这是临时 root：**重启后失效**，需要重新启动 Stellar 并执行。越狱过程可能失败或导致设备重启，请先备份重要数据，仅用于自己的设备。

## 当前版本

- 默认 `su` 入口修复，供无法自定义 su 路径的软件使用；每个应用仍需单独获得 root 授权。
- 兼容从 1.8 延续的已运行环境，修复时自动匹配当前内核对应的管理器。
- Material 3 界面跟随系统动态颜色与深浅色。
- 日志页支持一键分享 UTF-8 TXT，文件保存至 `Download/OneKeyJB`。
- SukiSU 配套版本为 v4.2.1；保留准备检查、root 诊断与免费说明。

## 开始使用

1. 下载并安装 APK，以及上表中对应的官方管理器。
2. 在手机开启无线调试，按 Stellar 的提示启动服务。
3. 打开本应用，连接 Stellar 并授予权限，选择配套管理器。
4. 点击「检查准备（只读）」，确认通过后点击「开始越狱」。已有 root 时会显示「修复 root 环境」。
5. 日志提示环境检查通过后，在当前内核对应的管理器里授权目标软件，彻底退出该软件再打开。

**Stellar 权限和 root 权限不同**，不能互相替代。需要验证本应用时，先给本应用 root 授权，再点击「验证 root」。

## 已有 root，但软件无法使用

保持 Stellar 运行，打开本应用点击「修复 root 环境」。修复会自动匹配已加载的内核，不要求先重新越狱。

例如，手机仍运行 1.8 留下的 KernelSU-Next 时，修复会使用 KernelSU-Next。若要切换到 SukiSU，需要先重启，再按所选管理器重新执行。

修复完成后，在当前管理器中检查目标软件的授权，彻底关闭并重新打开。某个软件通过授权不代表其他软件也已通过；存储目录访问还与软件自身权限和挂载空间有关。

## 分享日志

进入「日志」页，点击「分享 TXT」，从系统分享面板选择接收应用。文件也会保存在 `Download/OneKeyJB`，空日志不会导出。

反馈问题时请同时说明 App 版本、设备内核、当前使用的管理器和出现问题的软件。

## 已验证范围

v2.3.3 已在运行旧版 KernelSU-Next 的 OnePlus 16 上验证修复、默认 su 的授权与拒绝、命令和管道、动态颜色及 TXT 导出。

本版未重启重新验证完整越狱过程，也未逐一验证所有第三方软件；SukiSU 路径仍标为实验性。

## 作者与第三方项目

作者：**星苒鸭** · [GitHub](https://github.com/xingranya) · [xran.uk](https://xran.uk)

感谢 [KernelSU-Next](https://github.com/KernelSU-Next/KernelSU-Next)、[SukiSU Ultra](https://github.com/SukiSU-Ultra/SukiSU-Ultra) 与 [Stellar](https://github.com/roro2239/Stellar)。第三方组件的许可证以各自项目为准；本仓库保留 [LICENSE](LICENSE)。
