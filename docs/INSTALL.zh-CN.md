# 轻栈 PinoraDesk 1.0.0 安装说明

仅Apple Silicon Mac（ARM64），配置macOS14+；本机开发验证为macOS15.2 ARM64。Intel与Windows暂无包。应用内版本1.0.0，标签v1.0.0。

## 下载

从[版本页](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/tag/v1.0.0)选择[PinoraDesk.dmg](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/PinoraDesk.dmg)或[PinoraDesk.zip](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/PinoraDesk.zip)。自动生成的Source code不是应用。版本和附件未展示时请勿把旧包改名代替。

## 安装或升级

1. 保存正在处理的JSON／图片，并备份需要保留的数据。
2. 从菜单栏真正退出旧轻栈，关闭窗口仅隐藏，不要覆盖正在运行的App。
3. DMG中将App拖入Applications；ZIP完整解压后将App放进应用程序。
4. 打开同一位置的App，检查版本和原有设置。不要同时运行多个目录中的副本。
5. 截图按macOS正常屏幕录制授权流程操作；系统要求退出时退出再打开。

本包沿用固定本地开发签名、未经Apple公证；不声称完成跨机器安装升级验收。首次打开只采用系统提供的单应用放行流程。恶意软件／损坏提示不要当普通验证提示绕过，不关闭整机保护，不重置其他应用权限。

## 完整性核对

下载同版本SHA256SUMS.txt，在保存安装包的目录运行：

```sh
shasum -a 256 PinoraDesk.dmg
```

与校验文件同名条目比对。不同则停止使用并重新下载。摘要相同不等于Apple公证或无缺陷。

## 更新和卸载

1.0.0设置页有手动更新流程，但尚未配置真实可信清单，请使用公开版本页下载。下载不自动安装；更新前真正退出并保留旧包／备份。卸载App不自动删除本机数据；清理前在对应数据维护入口确认目标。

[完整使用手册](USER_GUIDE.zh-CN.md) · [FAQ](FAQ.zh-CN.md) · [验证范围](VERIFICATION_1.0.0.md)
