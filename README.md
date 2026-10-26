# 轻词 · QingDict

常驻 macOS 菜单栏的轻量词典。按 **Option + Space** 打开图标下方的查词浮窗，输入时显示本地候选词，用上下键和回车，或鼠标点击查询。

## 安装

```sh
brew install --cask etanxing/tap/qingdict
```

也可以从 [Releases](https://github.com/etanxing/qingdict-releases/releases/latest) 下载 ZIP，解压后将 `轻词.app` 拖到“应用程序”文件夹。

需要 Apple Silicon Mac、macOS 13 或更新版本。暂不支持 Intel Mac。本地释义和输入补全可离线使用，有道在线内容和发音需要网络连接。

目前使用临时签名，尚未通过 Apple 公证。首次打开若被 macOS 拦截，请先尝试打开应用，再到“系统设置 → 隐私与安全性”查看并手动允许。无需关闭系统安全保护。

## 功能

- 优先显示本机 macOS 牛津英汉汉英词典的释义，再追加有道在线内容；系统词典未就绪或未命中时，使用内置 ECDICT 的 50,000 常用词英汉词库。
- 输入时显示最多 8 个本地补全候选和简短释义，支持键盘和鼠标选择。中文输入法组词时暂停补全。
- 菜单栏小窗宽度固定，初始只显示搜索框、设置与退出；查询时向下展开。
- 可切换到普通独立窗口，支持调整大小、最小化和全屏。大小窗互斥，保留当前查询。
- App 字体与字典字体分别调整，设置保存在本机。
- 有道英汉、汉英、英英、柯林斯双解、同根词、专业释义和例句等内容。
- 点击词典区块标题展开或折叠，支持“显示全部 / 折叠全部”。
- 英式、美式发音按钮和音标。
- 最近查询、关于窗口、可选开机启动。
- Esc 先收起候选列表，再按一次收起小窗；Option + Space 唤出或收起小窗，右击菜单栏图标可退出。

使用 macOS 牛津词典时，可从“设置 → 打开 macOS 词典”进入系统词典设置，下载并启用“牛津英汉汉英词典”。轻词不复制或重新分发 Apple 词库。

## 更新与卸载

```sh
brew update
brew upgrade --cask etanxing/tap/qingdict
brew uninstall --cask qingdict
```

## 数据与反馈

仅在回车或点击候选确认查询后，向有道发送所选单词或短语；输入补全和本地释义不需要联网。发音按钮会向有道请求对应音频。最近查询保存在本机，可在设置中清空。有道在线接口不可用时仍保留本地释义。

内置 ECDICT 词库来自 [skywind3000/ECDICT](https://github.com/skywind3000/ECDICT)，MIT 许可与来源说明随安装包提供。

通过本仓库的 [Issues](https://github.com/etanxing/qingdict-releases/issues) 反馈问题。

本仓库仅提供安装包、版本说明和问题反馈，应用源码不公开。
