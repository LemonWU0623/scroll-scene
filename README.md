# Scroll Scene · 滚动转场

一个给 Codex 用的网站设计 skill。访客向下滚，镜头就向前走；滚回来，画面沿原路倒带。转场从网站自己的内容里挑：建筑案例可以穿过改造前的拱门，看见完工后的庭院；字体作品集可以穿过字母 O，让字腔里的一小块纹理展开成整张海报。

## 先看效果

下载仓库，用浏览器打开 [assets/scroll-portal.html](assets/scroll-portal.html)。慢慢向下滚，留意字母 O 里的两种印色。停手或往回滚，可以逐帧查看从字腔到海报的过渡。示例是一个独立 HTML 文件，支持键盘滚动；开启系统的「减少动态效果」后，两幕会按阅读顺序排列。

## 安装到 Codex

在 macOS 或 Linux 终端运行：

```sh
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
git clone https://github.com/LemonWU0623/scroll-scene.git "${CODEX_HOME:-$HOME/.codex}/skills/scroll-scene"
```

也可以下载 ZIP，解压后将包含 `SKILL.md` 的文件夹命名为 `scroll-scene`，放进 Codex 的个人 `skills` 目录。

## 用在自己的网站

在 Codex 中打开网站项目，输入：

> 用 $scroll-scene 改我的作品集首页。从已有作品里挑一个物件，让下一件作品的细节先出现在它里面，再让滚动带着访客穿过去。做好后给我一个可以试玩的预览。

也可以指定镜头的起点和落点：

> 用 $scroll-scene 做建筑改造案例的开场。从旧立面穿过拱门，停在新庭院的完工照，接着就是项目正文。

镜头设计、进度映射和浏览器验收方法见 [SKILL.md](SKILL.md)。
