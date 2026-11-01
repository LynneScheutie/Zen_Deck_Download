<div align="center">

# Zen Deck

优绩主义防内耗机器

把日常该做的事做成卡池，抽一张就去做一张

**本仓库仅存放安装包，不包含源代码。**

</div>

---

## 这是什么

一个让你从「今天没干正事」的焦虑里抽身的抽卡工具。抽到什么算什么，抽到稀有的算赚到，抽到普通的也不用自责——反正牌是随机发的，不是你选的。

- **抽卡**：2500 张防内耗任务卡，单抽与十连，十连动画平滑
- **自习室**：番茄钟专注计时 + 内置音乐，可循环、随机、单曲
- **歌单二**：把本地音乐直接拖进窗口即可加入，重启后还在
- **图鉴**：收集与清空，清空需二次确认
- **完全本地**：断网可用，无广告，不收集任何数据

## 下载

| 平台 | 版本 | 安装包 |
| --- | --- | --- |
| macOS | **4.2** | [Zen-Deck-4.2.dmg](https://github.com/LynneScheutie/Zen_Deck-download/releases/download/macOS-v4.2/Zen-Deck-4.2.dmg) · 35 MB |
| Windows | **4.2** | [Zen-Deck-4.2-Windows.zip](https://github.com/LynneScheutie/Zen_Deck-download/releases/download/Windows-v4.2/Zen-Deck-4.2-Windows.zip) · 157 MB |

旧版本留在 [Releases](../../releases) 里：

| 平台 | 版本 | 安装包 | 说明 |
| --- | --- | --- | --- |
| macOS | 4.1.1 | [Zen-Deck-4.1.1.dmg](https://github.com/LynneScheutie/Zen_Deck-download/releases/download/macOS-v4.1.1/Zen-Deck-4.1.1.dmg) · 20 MB | |
| Windows | 4.1.1 | [Zen-Deck-4.1.1-Windows.zip](https://github.com/LynneScheutie/Zen_Deck-download/releases/download/Windows-v4.1.1/Zen-Deck-4.1.1-Windows.zip) · 143 MB | |
| macOS | 3.2 | [Zen-Deck-3.2.dmg](https://github.com/LynneScheutie/Zen_Deck-download/releases/download/macOS-v3.2/Zen-Deck-3.2.dmg) · 75 MB | 改名前的最后一版，见下方说明 |

## 安装

### macOS

1. 下载 `.dmg` 后双击打开，把应用拖进「应用程序」文件夹。
2. 应用未经 Apple 公证，首次打开会提示「无法验证开发者」。到「系统设置 → 隐私与安全性」，在下方点「仍要打开」，再确认一次。
3. 如果提示「文件已损坏」，在终端执行下面这行再打开：

```bash
xattr -dr com.apple.quarantine /Applications/"Zen Deck.app"
```

macOS 版内置了独立的运行环境，**不需要另外安装 Python**，要求 macOS 12.0 及以上。

### Windows

1. 把整个 `Zen Deck-win64` 文件夹解压出来，**不要只拖出 exe**，程序依赖同目录下的其他文件。
2. 双击 `Zen Deck.exe` 即可运行，无需安装。
3. 首次打开会弹「Windows 已保护你的电脑」，点「更多信息」→「仍要运行」。这是未签名软件的正常提示。
4. 卸载就是删掉整个文件夹，不写系统、不留残留。

> [!NOTE]
> 从 3.2 升级到 4.x 时，应用名称从「优绩主义防内耗机器」改成了「Zen Deck」。macOS 上升级后建议先把旧版拖出「应用程序」，避免新旧两个图标并存。图鉴进度保存在应用本地存储中，换应用名等于换了存储位置，**旧进度不会自动带过来**。

## 校验值

| 文件 | SHA-256 |
| --- | --- |
| `Zen-Deck-4.2.dmg` | `737d4ce3ef8260305a9c1723ce32ef0dbb986f711badce55212dbcce2b7cb844` |
| `Zen-Deck-4.2-Windows.zip` | `9d26f36a8dac1f8489930b2d77ce9c6ea3086b34811cdaea89750cb6c020f34c` |
| `Zen-Deck-4.1.1.dmg` | `51eeef43549d337ab9ce1e4347aa11fceeb215f9bb61c37d17ab098bcba7039e` |
| `Zen-Deck-4.1.1-Windows.zip` | `9c3aa60fef2c2a21b1bc70bc2ad7e11b52bf12328b9ff191d6754f3634f7ff62` |
| `Zen-Deck-3.2.dmg` | `746cc99eb6971e376a689f7bc239fb7b242bd5c23e42f23e495fb88b1a063a94` |

macOS 上执行 `shasum -a 256 文件名`，Windows 上执行 `certutil -hashfile 文件名 SHA256`。

## 关于源代码

源代码未公开，本仓库也不含任何源文件。

可以自由使用本软件，但不允许反编译、二次打包后以自己的名义分发，也不允许剥离版权声明。

## 问题反馈

在 [Issues](../../issues) 里提交，请说明系统版本、软件版本，以及具体在做什么操作时出的问题。
