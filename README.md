# Luker 2.7.0 GPT 生图版

手机端请直接安装原生 APK，不需要再安装 SillyTavern 第三方扩展：

[下载 Luker GPT 生图版 APK](https://github.com/shuiyue698/sillytavern-gpt-image-relay/releases/latest)

- 版本：`2.7.0-gpt.3`
- 文件：`Luker-GPT-Image-v2.7.0-gpt.3-arm64.apk`
- 独立包名：`com.luker.gptimage`，可以与官方 Luker 同时安装
- 完整构建说明见 [`apk/README.md`](apk/README.md)

## 旧版第三方扩展源码

下面内容仅供需要普通 SillyTavern 扩展的用户参考。安装上面的原生 APK 后，不需要再安装此扩展。

### GPT 生图中转站（SillyTavern）

这是普通 SillyTavern/Luker 使用的第三方扩展版，不是 TauriTavern 专用扩展。仓库根目录就是标准 ST 扩展入口，可直接用 Git 安装。

## 安装

在 SillyTavern 的第三方扩展 Git 安装入口填入：

```text
https://github.com/shuiyue698/sillytavern-gpt-image-relay.git
```

也可以下载 `sillytavern-gpt-image-relay-v1.1.9.zip`，解压到 `public/scripts/extensions/third-party/sillytavern-gpt-image-relay`。

安装或更新后，先删除/停用旧的 TauriTavern 版和其他旧 GPT 生图扩展，再完整重新加载页面。不要把 `sillytavern-mobile-patch` 根仓库当作普通第三方扩展安装。

扩展会优先使用支持自定义中转站的同源代理接口，并自动回退为直接访问中转站。若手机 WebView 报 CORS 错误，需要在中转站允许当前酒馆来源，或给 SillyTavern/Luker 服务端安装对应代理补丁。

功能包括角色、场景、最后一段生图按钮，自定义端点和 Key，模型/分辨率/风格选择，参考图上传、自动分析及可编辑结果。分析和生图会读取左侧当前选择的“自定义（兼容 OpenAI）”端点；面板按钮固定在手机输入框上方，并可拖动面板。
