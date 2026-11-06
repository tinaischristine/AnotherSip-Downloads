# Another Sip 1.0.0

首个公开下载版本。

## 功能

- 原生 macOS SwiftUI App 与 WidgetKit 桌面小组件
- Small 与 Medium 两种尺寸
- 1–12 个可自定义阶段
- 可编辑 Emoji、名称、开始与结束时间
- 可添加、删除、调整顺序并恢复五阶段默认预设
- 阶段不能重叠，允许保留空档
- 当前阶段或下一阶段的分钟级倒计时
- 浅色、深色、跟随系统主题与 12/24 小时制
- 本地保存、完全离线

## 系统与分发

- macOS 14.0 或更高版本
- Universal Binary：Apple Silicon `arm64` + Intel `x86_64`
- ad-hoc 签名，无 Developer ID，无 Apple 公证
- 不依赖个人 Provisioning Profile，没有 7 天到期问题
- 首次运行需要在“系统设置 → 隐私与安全性”中对 Another Sip 单独点击“仍要打开”

## 验证范围

- Release 构建成功
- 12 项 XCTest 全部通过
- 主 App 与 Widget Extension 嵌套签名严格验证通过
- 主 App 与 Widget Extension 均验证为 `arm64 + x86_64`

当前版本尚未在另一台 Mac 上完成首次安装、安全授权和小组件列表的实机验证，因此不对此作成功声明。
