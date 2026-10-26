# 轻词 · QingDict

常驻 macOS 菜单栏的在线词典。按 **Option + Space** 打开图标下方的查词浮窗，输入单词后按回车。

## 安装

```sh
brew install --cask etanxing/tap/qingdict
```

也可以从 [Releases](https://github.com/etanxing/qingdict-releases/releases/latest) 下载 ZIP，解压后将 `轻词.app` 拖到“应用程序”文件夹。

需要 Apple Silicon Mac、macOS 13 或更新版本及网络连接。暂不支持 Intel Mac。

目前使用临时签名，尚未通过 Apple 公证。首次打开若被 macOS 拦截，请先尝试打开应用，再到“系统设置 → 隐私与安全性”查看并手动允许。无需关闭系统安全保护。

## 功能

- 有道英汉、汉英、英英、柯林斯双解、同根词、专业释义和例句等内容。
- 点击词典区块标题展开或折叠，支持“显示全部 / 折叠全部”。
- 英式、美式发音按钮和音标。
- 最近查询、窗口置顶、可选开机启动。
- Esc 或再次按 Option + Space 收起窗口；右击菜单栏图标退出。

## 更新与卸载

```sh
brew update
brew upgrade --cask etanxing/tap/qingdict
brew uninstall --cask qingdict
```

## 数据与反馈

查询时向有道发送输入的单词或短语；发音按钮会向有道请求对应音频。最近查询保存在本机，可在设置中清空。有道在线接口发生变化或不可用时，查词可能受影响。

通过本仓库的 [Issues](https://github.com/etanxing/qingdict-releases/issues) 反馈问题。

本仓库仅提供安装包、版本说明和问题反馈，应用源码不公开。
