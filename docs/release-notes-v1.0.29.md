# PS 切图工具 v1.0.29

## 本版修复

- 修复部分 macOS Photoshop 环境中校对窗口缩略图显示为灰色占位块的问题。
- 兼容 Photoshop Imaging API 返回字符串、数值字节数组和严格 ArrayBuffer 的不同宿主实现。
- 去除 macOS UXP 原生按钮外观对预览边界框和校对操作栏的覆盖。

## 验证

- 自动化测试：176/176 通过。
- Adobe UXP CLI Manifest 校验通过。
- Photoshop 27.8.0 加载验证通过。

## 安装包校验

- 文件：`com.tu.ps-slicer_PS.ccx`
- 大小：`67,989 bytes`
- SHA-256：`EBD57DD67F8286519F6911DC4488492048558FF87D4B79CDB182CDF64206D649`
