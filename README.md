# 樱按钮 / みこボタン / Miko Button

## 请注意

### 此仓库仅用于测试新功能，包含部分实验特性，可能会产生各种不可意料的错误，请勿在生产环境使用！

### 可用于公开使用的稳定版本：[MikoButton](https://github.com/VoiceButtonUnitedProject/MikoButton)

### Nya Hello ~!

### https://sakuramiko.org

相关链接 / 関連URL / Related Links:

* [Sakura Miko's Youtube channel](https://www.youtube.com/channel/UC-hM6YJuNYVAmUWxeIr9FeA)

* [Sakura Miko's Twitter](https://twitter.com/sakuramiko35)

## 参与完善本项目

**Rome was not built in a day.** 

欢迎参与完善这个并不成熟的项目，或者为我们提出宝贵的意见！

联系方式：[Telegram 群组](https://t.me/mikobutton)  or Email: `hello@sakuramiko.org`

请 Fork 本项目进行修改，完成修改后在本项目中发起一个 Pull Request。

### 添加或修改音频

**简述**：所有的音频信息都存储在 [src/voices.json](src/voices.json) 中，要添加或修改音频，你需要同时修改对应的文件。

音频一律为mp3格式，存储在 [public/voices](public/voices) 中。对应的URL为 `voices/`。

添加的新音频请先使用类似 MP3GainGUI 的软件进行音量标准化，目前音量全部标准化为80。

由于本项目采用强缓存策略，除 `index.html` 外，文件名一致的文件，即使做出修改也 **永远** 不会被客户端刷新。因此新添加的音频，无论是新增还是修改，文件名都 **必须** 和之前任何文件名不同。

修改音频之后请删除原音频文件。

### 参与翻译

主程序翻译在 [src/locales](src/locales) 中的三个以语言名命名的 js 文件中。

语音的翻译在 [src/voices.json](src/voices.json) 中。

## 部署本地开发环境

本项目是使用 Vue + jQuery + Bootstrap 3 开发的。

要部署本地开发环境，请首先安装最新版本的 Node 和 Yarn 包管理器。然后，请按照下列步骤操作：

1.Fork 并 Clone 代码到本地。

2.进入代码所在目录，运行 `yarn` 安装依赖。

3.运行 `yarn serve`，启动本地开发服务器，项目将被临时部署在 `localhost:8080` 上。在代码修改过程中，本地开发服务器可以即时更新修改结果。

4.要编译可用于部署的文件，请运行 `yarn build`，这将在 `dist` 目录生成完全静态的文件。编译完成后，您可以直接将整个 `dist` 目录部署至 Github Pages 等静态文件托管服务上。

## LICENSE

This project is modified based on the [Mio button](https://github.com/VoiceButtonUnitedProject/MioButton).

程序部分: MIT

音频部分: [hololive 二次创作条款](https://www.hololive.tv/terms)

本项目为爱好者作品，与 hololive 官方没有关联。

## 特别感谢

[![Vercel Logo](https://cdn.jsdelivr.net/gh/paizi/vue-test/vercel.svg)](https://vercel.com)

本项目由 [Vercel](https://vercel.com/) 强力驱动。

以及所有支持这个项目的朋友，你们的鼓励是我孜孜不倦的源动力，谢谢你们。

虚位以待...