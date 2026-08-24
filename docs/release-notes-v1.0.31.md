# PS 切图工具 v1.0.31

## 本版修复

- 校对缩略图优先使用标准透明 PNG 的 UXP `ImageBlob` 对象 URL，避免不同 Photoshop 宿主对临时路径或 Imaging 编码的差异。
- 预览点击层改为透明非原生按钮元素，修复 Windows/macOS UXP 原生按钮皮肤遮挡缩略图、只显示灰色圆角占位的问题。
- 保留 PNG Data URL、Photoshop 编码和原始 ImageBlob 回退；缩略图资源在结果刷新和关闭校对时释放。
- 预览结果仍支持鼠标点击及 Enter/Space 键盘选择，图片层和点击层保持独立，蓝色边界框不偏移。

## 验证

- 自动化测试：180/180 通过。
- 项目结构检查通过。
- Adobe UXP CLI Manifest 校验与 CCX 打包通过。
- Photoshop 27.8.0 开发加载验证通过。

## 安装包校验

- 文件：`com.tu.ps-slicer_PS.ccx`
- 大小：`70,008 bytes`
- SHA-256：`7CB7BB0716D10B2DAE5F0F40C7FD8A9DD4E145E4C8C2718247700475AE0D8EE3`

本环境没有可操作的 macOS Photoshop，未将本版描述为完成 macOS 实机视觉验收；建议安装后在目标 Windows/macOS 版本确认缩略图和点击操作。
