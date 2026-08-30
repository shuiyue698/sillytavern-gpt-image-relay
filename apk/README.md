# Luker 2.7.0 GPT 生图版 APK

这是基于官方 `funnycups/Luker@v2.7.0` 制作的 Android arm64 原生生图版。

- 应用名称：`Luker GPT 生图版`
- 版本：`2.7.0-gpt.1`
- 独立包名：`com.luker.gptimage`
- 可以和官方 Luker 同时安装
- 生图功能已经内置，不需要安装 SillyTavern 第三方扩展

APK 在仓库的 Releases 页面下载，文件名为：

`Luker-GPT-Image-v2.7.0-gpt.1-arm64.apk`

## 内置功能

- 按角色、场景、最后一段文字生成图片
- 自定义中转站 API URL 和 Key
- 连接测试及模型列表读取
- 独立选择生图模型、分析模型、分辨率和画风
- 上传、清除和自动分析参考图
- 编辑参考图分析结果
- 将生成图片保存到对应聊天消息的图片记录

## 构建来源

`luker-native-gpt-image-v2.7.0.patch` 是叠加在官方 `v2.7.0` 标签上的完整源码补丁。GitHub Actions 会重新拉取官方源码、应用补丁并构建 APK。

