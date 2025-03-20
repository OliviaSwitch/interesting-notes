---
tags:
  - "#obsidian插件"
  - "#剪藏"
connect-url: https://sspai.com/post/97131
---
2024 年是我做 PPT 最多的一年。

这一年里面我开了不知道多少次各种会议，做了无数次汇报。这些要求的汇报不仅强行撼动了我的社恐本性，还给我带来了一大堆需要做的 PPT。在和 PowerPoint 无奈共事一年后，我产生了一个思考：有没有比直接在 PowerPoint 中手搓 PPT 更高效的 PPT 制作方法呢？

## PowerPoint 到底哪里不好？

![](https://cdnfile.sspai.com/2025/03/08/article/02d372d85937b7ee86f46dc0ad268fda.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

PowerPoint、WPS、Keynote 是我们最常用的演示制作软件。这些软件制作 PPT 的思路都是「所见即所得」，即在一块画布上「画出」我们需要的页面。这种思路的好处是上手非常简单，上限也非常高。一个没有任何经验的人也可以轻松通过套模板用 PowerPoint 做出个还像样的 PPT；而一个高手则可以用 PowerPoint 做各种复杂的设计。但是经过大量汇报的考验之后，我发现 PowerPoint 有其自己的问题：

- PowerPoint 的排版手段太过灵活，对于高手来说这是优点；但是对于没有设计本领的我来说，就很容易排出混乱丑陋的版面；
- PowerPoint 的排版方式比较复杂，即使有模板的帮助，也需要用大量的精力应付排版，让我不能完全专注于内容；
- 我的汇报内容经常涉及到数学公式，PowerPoint 的公式继承了 Office 全家桶的公式系统，体验很差。

用 AI 制作 PPT 兴起之后，我试用过一些基于 AI 的 PPT 生成器。它们速度极快，而且可以保持风格的一致，乍一看让人觉得很惊艳；然而仔细查看就会发现，AI 生成的 PPT 虚有其表，不论内容还是排版细节都禁不起推敲。因此短期内仍然不能指望 AI 完全代劳，我仍然需要一个更好的 PPT 制作方法，我希望这个方法可以：

- 提供一定的框架，让我不需要太关注排版的问题就可以做出风格一致、简练明晰的 PPT；
- 有更高效的公式书写方式。

## 探索

首先来看第一个需求：

> 提供一定的框架，让我不需要太关注排版的问题就可以做出风格一致、简练明晰的 PPT。

有没有觉得，这和 Markdown 的优势很相似？

- 通过**限制排版手段的灵活性**，Markdown 保证了排版效果下限，任何人都可以轻易排版出风格一致且具有简约美的文章；
- Markdown 排版方法极为简单，保证我们可以将精力集中在文章内容上。

正巧，现在大多数 Markdown 编辑器都支持 LaTeX 数学公式，可以满足第二个需求。在这样的情况下，我自然而然地打起了用 Markdown 排版 PPT 的主意。

用 Markdown 做 PPT 的体验究竟怎么样？为了回答这个问题，这段时间里我体验了多个可以基于 Markdown 生成 PPT 的工具，以下是我的记录。

## Obsidian 幻灯片

我是个重度 Obsidian 用户，首先就想到 **Obsidian 原厂自带的核心插件就支持以 PPT 形式演示自己的笔记**。要用 Obsidian 将笔记转化为幻灯片，只需要先打开核心插件「幻灯片」，写一篇 Markdown 笔记，然后在需要分页的地方用`---`隔开，就可以产生熟悉的分页形式 PPT 了。 

![](https://cdnfile.sspai.com/2025/03/08/article/6d0276ef12636c83df87b1a26ac365cf.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/15c52dbc6aa31b74bebf52a6ec1f5159.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

最后打开命令面板，选择「幻灯片：开始演示」，Obsidian 就会将笔记渲染为演示形式，这样你就可以轻松演示自己的文章了。 

![](https://cdnfile.sspai.com/2025/03/08/article/6c3936f0cce6bb8902cee6dd0b08645c.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/806be9ff359c6a2bde832c7085953182.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/4934b9bc304abf53397e2ad35755afe8.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

然而这个演示的排版效果似乎不如人意。我相信，应该不会有人喜欢这种全文居中、字体浮夸的 PPT。

更致命的是，我上下翻找一圈没有找到任何幻灯片自定义设置，也没有找到「导出为 PPT」这个选项；这意味着。Obsidian 的幻灯片插件仍然停留在一个概念性功能的层次，还不适合真正投入应用。

## Marp

由于核心插件幻灯片不如人意，所以第三方插件市场出现了一些 PPT 插件，其中比较著名的是基于 Marp 的 Markdown 转 PPT 插件。

![](https://cdnfile.sspai.com/2025/03/08/article/0623576f91ef809cbd113c3fac79d711.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

相比起核心插件幻灯片，Marp Slides 支持实时预览，并且提供了丰富的导出选项（支持导出为PPT、PDF、PNG）。实时预览这个特性让我们可以实时地调整每一页内容的多少，不需要像幻灯片插件一样，整体演示的时候才知道哪些页面内容溢出了。 

![](https://cdnfile.sspai.com/2025/03/08/article/c6745773d5ad8451a19973ecffb44b91.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/3cc5dab514017c3ad00d3b4d8703aa2f.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/990058ece9835d0337a841fb82b12023.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/5141999ddd500c13c40b01d57ac9044f.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

Marp Slides 支持使用自定义主题。只需要下载你需要的主题`.scss`文件，之后在属性中选择使用的主题即可。

![](https://cdnfile.sspai.com/2025/03/08/article/133ac233be31eacc99e8fff58b88602b.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

使用主题后的效果：

![](https://cdnfile.sspai.com/2025/03/08/article/00f8ed80a69200f4ff038997dc7a6e04.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

我这里使用的主题来自 [Awesome Marp](https://sspai.com/link?target=https%3A%2F%2Fgithub.com%2Ffavourhong%2FAwesome-Marp)，其提供了一整套相关 Marp 主题，并且配合 Marp 的特殊 Markdown 语法可以做出样式丰富、风格统一的 PPT。由于我只想在 PPT 上偷懒，我提供的案例并不能显露出 Marp 排版以及 Awesome Marp 的强大能力，这里我直接援引 Awesome Marp 作者的 PPT 展示：

![](https://cdnfile.sspai.com/2025/03/08/article/f03ca8b35c5389d83d3f9d313152a297.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/aa6b2c65604a552f82c15f20e6221f04.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/c88ffe1d112c503d4f86e6481e18ed98.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

就我个人体验而言，Marp Slides 有一个比较严重的 bug，那就是在尚未配置好导出选项的时候按下右上角四个键会**一键删除当前文件**。如果没有备份机制的话，这样的 bug 会造成一定的损失。由此可见，这个插件尚不算非常完善，有待后续进一步更新。 

![](https://cdnfile.sspai.com/2025/03/08/article/230998c054d0ad1c73fcbe20c6ad1bbc.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/cfc8a363409499be31eb3759c594cce5.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

在我看来，不论是安全起见还是插件体验，Marp 的 VSCode 插件都相对更加适合于完成这个任务。不过需要注意的是，**Marp Sildes 和 Marp VSCode 都会直接导出位图 PPT 文件**，即导出的 .pptx 文件不支持再用 PowerPoint 修改，而且清晰度可能达不到你的要求。想要入手 Marp 的读者务必好好考虑这一点。

![](https://cdnfile.sspai.com/2025/03/08/article/9a2a37e5645ae2858de58c2252e60ac9.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

## Slidev

Marp 支持的玩法很多，Slidev 则是 Marp 的威力加强版。如果你没有前端基础，也不想折腾的话，可以直接跳过这一章节。

Slidev 和 Marp 一样，用 YAML 头指定属性，用`---`分隔页面。不过 Slidev 不仅支持的属性更多，还可以在幻灯片中插入一些代码来控制其行为。在本地使用 Slidev 需要 Node.js 环境，并且先用 npm 生成项目：

```
npm init slidev@latest
```

生成项目之后，我们通过编辑`slides.md`来制作幻灯片。在你编辑好之后，通过`slidev`可以启动本地服务器，在`http://localhost:<port>`预览自己的PPT。

Slidev 的语法是相对比较复杂的。相比 Marp，Slidev 可以说已经把 Markdown 改得面目全非了。在 Slidev，你可以直接用 HTML 语法在页面中自定义可交互按钮： 

![](https://cdnfile.sspai.com/2025/03/08/article/4bb2a7c3d4e53dd607cf6df03952d9c4.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/03/08/article/e9b8ff127aa596dde1ce52f458e32992.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

> 由于本人做的实例太丑，所以这里采用了官方的实例做展示。

在`slides.md`中自定义 CSS，实现一级标题的渐变色标题效果：

```
<style>
h1
 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);  
  background-size: 100%;  
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>
```

![](https://cdnfile.sspai.com/2025/03/08/article/7cc2c49e60d05a534114b3e7b41d2f8c.png?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1/format/webp)

Slidev 的强项是**代码显示以及代码动画**。通过 shiki-magic-move，Slidev 可以实现 PowerPoint 都很难实现的代码动画：

![](https://cdnfile.sspai.com/2025/03/08/article/0e6e8030b9e352af9d79b1843046dedb.gif)

可以想见，如果能够在会议或者课程上面使用这样的动画演示自己的代码可以带来多么惊艳的效果。更重要的是，在 Slidev 中制作这样的动画非常容易。我们不需要考虑字段如何移动，只需要将变化前后的代码按步骤列为一组 Markdown 代码块，Shiki 会自动考虑如何产生动画效果。

![](https://cdnfile.sspai.com/2025/03/08/article/4cca66114c57ea5a517d2a2fbd644d92.gif)

Slidev 是一个高度专业化并且可自定义的 Markdown 转 PPT 解决方案。相比 Marp，Slidev 可以实现更多惊艳的特效以及交互元素。但是为了实现这些功能，Slidev 的上手难度直线上升，只适合部分专业需求以及具有计算机背景的人士。

此外，和 Marp 一样，Slidev 对导出的支持较差，导出的是不可用 PowerPoint 修改的位图 PPT，会失去所有动画效果，并且清晰度不高。Slidev 比较适合使用自己的笔记本进行录制演示，或者连接屏幕或投影仪后进行演讲，而不适合导出 .pptx 文件使用。

## 综合体验

经过我一段时间的体验，我对各个通过 Markdown 做幻灯片的软件评价如下：

- Obsidian 幻灯片：还是个半成品，有待进一步完善功能；
- Marp：比较好地平衡了可定制性和易上手程度，学习难度不高，可以为我们免去许多排版上的烦恼，帮助我们专心于内容创作。Marp 可以通过 VSCode 插件使用，也可以通过 Obsidian Slides 使用，但是我认为前者的开发成熟度更佳，更为推荐；
- Slidev：高度专业化，可以自定义一些特殊效果、动画以及交互组件；通过 shiki-magic-move 可以轻松制作出令人惊艳的代码动画，很适合用自己的电脑录制演示或者现场演示。但是相比之下学习成本较高，而且不适合导出使用；

和用 Markdown 写文章一样，使用 Markdown 排版幻灯片最大的好处就是可以**将注意力集中到内容上，而非排版上**。这反映了我一开始的愿望：节省精力。但是实际上，不论是 Marp 还是 Slidev 都具有比较高的可玩性，一不留神就很容易沉迷于各种配置以及惊艳的效果，反而失去本心。如果你的心态和我一样，那么一定要在配置这条路上适可而止。可以**花一些精力制作一个模板 Markdown 文件**，之后就尽可能复用这套模板去生成 PPT，这样才能避免落入无尽的折腾陷阱。