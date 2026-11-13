# 轻栈 · PinoraDesk 1.0.0

一个快捷键，打开应用、处理JSON、截图贴图、查找文件。

**[下载Mac应用](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/PinoraDesk.dmg) · [功能手册](docs/USER_GUIDE.zh-CN.md) · [安装说明](docs/INSTALL.zh-CN.md) · [常见问题](docs/FAQ.zh-CN.md)**

## 下载

| 设备／资料 | 入口 |
|---|---|
| Apple Silicon Mac / M系列 | [PinoraDesk.dmg](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/PinoraDesk.dmg) · [PinoraDesk.zip](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/PinoraDesk.zip) |
| Intel Mac／Windows | 暂无应用包；Windows暂停 |
| 完整说明 | [PDF手册](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/PinoraDesk_User_Guide_1.0.0.pdf) · [离线HTML](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/PinoraDesk_User_Guide_1.0.0.html) · [离线FAQ](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/PinoraDesk_FAQ_1.0.0.html) |
| 验证与版本 | [1.0.0版本页](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/tag/v1.0.0) · [SHA256SUMS](https://github.com/SleepyBytepp/pinoradesk-downloads/releases/download/v1.0.0/SHA256SUMS.txt) · [验证范围](docs/VERIFICATION_1.0.0.md) |

macOS14+为配置目标，开发验证设备为macOS15.2 ARM64。本包使用固定本地开发签名，未经Apple公证；跨机器安装与部分原生场景仍未验收。以版本页实际附件为准，GitHub的Source code不是应用。

## 能做什么

- **应用启动**：中文／拼音搜索、最近使用、托盘、Dock恢复、可配置快捷键。
- **JSON工作区**：格式化、压缩、对比、纠错、行号、折叠、固定全局查询和大工作区；文件模式每份最高256MiB，分段查看编辑。
- **截图与贴图**：自由框选、辅助线、标注、复制、PNG／JPEG、OCR、贴图管理、跨屏拖选与手动滚动长截图。
- **剪贴板与片段**：文本历史、手工片段；图片和文件为单独开启的会话历史。
- **文件查找**：系统文件名索引、授权目录后备扫描，以及明确允许后的正文检索、类型筛选、行号和上下文。
- **时间和小工具**：当前时间／时间戳、时区转换、计算器、UUID、Base64、桌面取色和常用目录。
- **插件**：声明式JSON、多资源ZIP、受限WASM文本工具及手动管理的签名来源。
- **设置迁移**：基础设置与手工片段导出、逐项预览导入、备份恢复。
- **手动更新**：客户端验签与下载流程已实现；真实可信清单尚未配置，请从版本页下载。

20个工具入口按JSON、截图与贴图、时间、文本与编码、计算、文件与系统、扩展分类。窗口可拖动／缩放，1.0.0取消标题栏下重复圆角边框。

## 快速上手

1. 下载DMG或应用ZIP，保存旧版内容并真正退出，再安装到应用程序。
2. 打开轻栈，通过菜单栏或已配置快捷键唤起。首次默认Option+Space，有冲突可改Control+Option+Space。
3. 输入工具名，例如JSON、截图、时间戳；上下键选择、Enter执行、Esc隐藏。
4. 截图按系统正常流程授权。剪贴板采集、截图记录、记住贴图和WASM默认关闭，按需开启。

## 说明与隐私

迁移包未加密，可能包含手工保存的敏感文本，请妥善保管。用户主动打开网页、检查插件源等操作会访问系统或网络；本地优先不表示所有操作都离线。反馈问题前请脱敏。

公开下载、源码私有：本仓库的公开资料不包括应用实现源码。不兼容uTools商店，不声称已完整复刻Snipaste。正式公证、Windows、Intel和全部真实设备验收尚未完成。

[本版变化](docs/RELEASE_NOTES_1.0.0.zh-CN.md) · [完整手册](docs/USER_GUIDE.zh-CN.md) · [FAQ](docs/FAQ.zh-CN.md) · [项目许可](LICENSE) · [第三方许可材料](THIRD_PARTY_NOTICES.txt) · [反馈问题](https://github.com/SleepyBytepp/pinoradesk-downloads/issues/new)
