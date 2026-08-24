# PS 切图工具 v1.0.30

## 本版修复

- 校对缩略图默认由插件内纯 JavaScript 编码为透明 PNG Data URL，不依赖 Windows 或 macOS Photoshop 的本地临时路径。
- 兼容透明图、不同宿主图片解码实现，以及 ImageBlob/宿主路径回退。
- 主面板将两步的“分析”与“校对”合并为“分析校对”，一次点击完成分析并打开校对分割结果窗口。
- 已有分析结果时，“分析校对”直接进入校对窗口；“切开”和“导出”仍自动复用分析计划。

## 验证

- 自动化测试：178/178 通过。
- 项目结构检查通过。
- Adobe UXP CLI Manifest 校验与 CCX 打包通过。
- Photoshop 27.8.0 开发加载验证通过。

## 安装包校验

- 文件：`com.tu.ps-slicer_PS.ccx`
- 大小：`69,805 bytes`
- SHA-256：`4E5F34A26A09816C51BF5B84902FBCFD644D57354815F36C32EE6264C3D64F26`

本版尚未在本环境实际操作 macOS Photoshop；实现和自动化测试覆盖跨宿主缩略图编码路径，建议安装后在目标 Windows/macOS 版本复核一次。
