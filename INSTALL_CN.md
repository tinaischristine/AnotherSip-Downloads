# Another Sip 中文安装指南

## 安装

1. 从 GitHub Releases 下载 `AnotherSip.zip`。
2. 双击 ZIP 解压。
3. 将 `Another Sip.app` 拖入 Finder 的“应用程序”文件夹。
4. 在“应用程序”中双击 Another Sip。

## 首次安全授权

此版本没有 Developer ID 和 Apple 公证，macOS 第一次运行时可能阻止打开：

1. 先双击 Another Sip，并关闭系统的阻止提示。
2. 打开“系统设置 → 隐私与安全性”。
3. 向下找到 Another Sip 被阻止的提示，点击“仍要打开”。
4. 使用 Touch ID 或 Mac 登录密码确认，再点击“打开”。

这是 Apple 官方提供的单个 App 例外授权。不要运行 `spctl --master-disable`，也不要全局关闭 Gatekeeper。

## 添加桌面小组件

1. 至少打开 Another Sip 一次。
2. 在 App 中确认或修改阶段，点击“保存并更新小组件”。
3. 在桌面空白处按住 Control 点击，选择“编辑小组件”。
4. 搜索 `Another Sip`，选择小号或中号并拖到桌面。
5. 之后可以关闭主 App，小组件仍由 macOS 运行。

如果列表里暂时没有 Another Sip，请确认 App 已放入“应用程序”，重新打开 App 一次，再重新进入“编辑小组件”。必要时注销并重新登录 macOS。

## 更新与校验

新版本发布后，下载新 ZIP 并替换“应用程序”中的旧 App。Release 同时提供 SHA-256 文件，可在“终端”的下载目录运行：

```bash
shasum -a 256 AnotherSip.zip
```

结果应与 `AnotherSip.zip.sha256` 中的值一致。
