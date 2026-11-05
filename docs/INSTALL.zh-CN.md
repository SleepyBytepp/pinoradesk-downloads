# 安装轻栈 Mac 开发预览版

版本标签：`v0.2.0-preview.1`；应用内版本：`0.2.0`。

## 选择正确文件

- 只提供 **Apple Silicon / M系列 Mac，ARM64** 应用。
- 配置目标为macOS14及以上；本机已验证macOS15.2 ARM64，其他版本仍待实测。
- Intel Mac和Windows暂未提供安装包。
- 从[版本页](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/tag/v0.2.0-preview.1)下载DMG或应用ZIP，不要将`Source code`或`Code → Download ZIP`当成应用。
- 应用由独立公开下载仓库提供，无需源码仓库权限。[下载链接或404排查](FAQ.zh-CN.md#download)。

## 使用DMG安装

1. 下载`PinoraDesk-0.2.0-preview.1-macos-arm64.dmg`，双击打开。
2. 把`PinoraDesk.app`拖到`Applications`，或拷贝到自己的“应用程序”目录。
3. 弹出磁盘映像，从“应用程序”打开轻栈；后续一直运行这一份副本。
4. 如果已有旧版在运行，先用轻栈菜单“退出轻栈”，再替换同一位置的应用；不要一边运行一边覆盖。

## 使用ZIP安装

1. 下载`PinoraDesk-0.2.0-preview.1-macos-arm64.zip`并完整解压。
2. 找到`PinoraDesk.app`，放入“应用程序”后打开。
3. 随包说明、许可资料可另行保留；无需把整个工程、Node、Rust或编译缓存一起安装。

## 首次打开

当前是本机开发签名、尚未公证的预览包。若macOS提示无法验证开发者，确认来源与完整性后，按[Apple正常的单应用放行步骤](FAQ.zh-CN.md#first-open)处理。若提示恶意软件、会损坏电脑或已损坏，不要关闭安全保护强行运行，先重新核对包并反馈提示。

首次配置默认`Option+Space`；也可以从菜单栏或Dock打开，再到设置修改。演示中的`Control+Option+Space`是开发设备个人配置。

## 截图权限与数据

截图需要系统正常屏幕录制授权，只允许正在运行的这一份轻栈。按系统要求真正退出并重新打开；关闭窗口通常只隐藏。[详细排查](FAQ.zh-CN.md#screen-permission)。

自动剪贴板采集、截图历史、贴图记住和WASM默认关闭。开启贴图记住会保存原图/原文及可编辑标注；备份可能包含这些内容，不等于脱敏图片。

## 文件完整性

同一版本页提供`SHA256SUMS.txt`。可在终端中对下载文件计算SHA-256，与校验文件相应一行比较，例如：

```sh
LC_ALL=C /usr/bin/shasum -a 256 PinoraDesk-0.2.0-preview.1-macos-arm64.dmg
```

校验一致仅说明文件与发布附件一致，不等于Apple公证或没有软件缺陷。若不一致，停止使用该下载副本并重新下载。

## 更新和卸载

更新前真正退出轻栈，备份需要保留的数据，再替换“应用程序”中的同一份App。当前没有自动更新机制，不要同时运行多个解压副本。

不再使用时先退出，再删除“应用程序”中的App。删除App不等于删除本机数据；如需清理数据，请使用应用提供的数据维护入口并核对目标，不要盲删Library目录或运行别人提供的清理命令。

## 已知范围

这不是已完成正式发行验收的稳定版。CI仍有Mac本地HTTPS夹具超时和Windows Rust lint问题；真实多屏、多Space、权限撤回、安装升级等矩阵未全部验收。应用包只在本机封装/解包/签名完整性层面核对，跨机器下载后的首次Gatekeeper与权限流程仍需实测。

[完整功能手册](USER_GUIDE.zh-CN.md) · [常见问题](FAQ.zh-CN.md) · [验证边界](VERIFICATION_0.2.0.md)
