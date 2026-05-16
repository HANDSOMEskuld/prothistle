---
title: 免费白嫖 | 用 Cloudflare 搭建个人博客（零成本、零代码）
published: 2026-05-16
description: 零成本、零代码，用 Cloudflare 搭建属于自己的个人博客。
image: "./cover.png"
tags: [Cloudflare, 博客, 部署, 免费, Astro]
category: 教程
draft: false
lang: zh-CN
---

## 0x00 为什么值得拥有一个自己的博客？

大家每天在 𝕏 上分享想法，为什么不建一个**完全属于自己的博客**呢？

**核心好处：**

- **额外收入**：无需额外创作，接入 Google AdSense 就能躺着赚展示广告费
- **完全自由**：想写什么、怎么排版、用什么风格，全由你说了算
- **长期价值**：AI 正在爬取全网内容，你的博客将成为个人数字资产，助力“赛博永生”

**一份内容，两份收益**。  
下面手把手教你**零服务器、零代码**，10 分钟部署一个漂亮的个人博客。

**效果展示：**

![](https://raw.githubusercontent.com/HANDSOMEskuld/pics/main/2026/20260503163329556.png)

## 0x01 推荐框架 & 主题

静态博客主流框架：**Astro、Hugo、Hexo、Next.js** 等，各有千秋。

我精选了几个高质量主题（可直接替换）：

- [hexo-theme-stellar](https://github.com/xaoxuu/hexo-theme-stellar)
- [hexo-theme-redefine](https://github.com/EvanNotFound/hexo-theme-redefine)
- **[Firefly](https://github.com/CuteLeaf/Firefly)** ← **我正在使用的**
- [astro-theme-pure](https://github.com/cworld1/astro-theme-pure)

本教程以 **Firefly**（基于 Astro + Fuwari）为例，清新、现代、配置丰富，非常推荐。

## 0x03 开始部署

### 1. 本地部署

每个项目或者每个主题，在他们的仓库里面都有介绍说明如何部署和安装。

大家不用写代码，也不用运行命令，直接把他们的安装步骤复制下来Vibe Coding。

比如下面我就直接把下面提示词直接丢给 AI 编程工具（Cursor / Claude 等），让他帮忙安装部署：

> [!note]- 提示词（点击展开）
> ```text
> 帮我在目录 E:\功成名就的杂草\blog 下部署 Firefly 主题：
> 
> Firefly 是一款基于 Astro 框架的现代化个人博客主题，清新美观且高度可定制。
> 
> 请严格按照以下步骤执行：
> 1. git clone https://github.com/CuteLeaf/Firefly.git
> 2. cd Firefly
> 3. pnpm install
> 4. pnpm dev（启动本地预览）
> 
> 完成后帮我修改 siteConfig.ts 中的名称、头像、描述等基础信息。
> ```

> 在本地运行成功之后，一些定制的细节，比如说你的名字、你的头像，还有你的文章，都可以让 AI 进行 Vibe Coding。
### 2. 推送到 GitHub

本地跑通后，再让 AI 帮你新建仓库并推送。

在 GitHub 新建一个仓库，然后复制仓库地址。

![](https://raw.githubusercontent.com/HANDSOMEskuld/pics/main/2026/20260503165605292.png)

同样的用 AI 编程工具，让 AI 帮你把这个项目上传到 GitHub 上面。

![](https://raw.githubusercontent.com/HANDSOMEskuld/pics/main/2026/20260503122029123.png)



### 3. Cloudflare 部署

- 打开 [Cloudflare Dashboard](https://dash.cloudflare.com)
- 左侧 → **Workers & Pages** → **Create application** → **Continue with GitHub**
- 选中你刚推送的仓库 → 自动识别构建命令 → 点击 **Deploy**

![](https://raw.githubusercontent.com/HANDSOMEskuld/pics/main/2026/20260503123110574.png)

## 0x04 常见问题处理

**首次部署失败很正常**，直接复制 Cloudflare 的错误日志丢给 AI 即可。

AI 帮你修复后，重新 push 到 GitHub，Cloudflare 会**自动重新部署**，无需额外操作。

比如下面，我就在部署失败之后，让 AI 帮我修复，并重新上传：

![](https://raw.githubusercontent.com/HANDSOMEskuld/pics/main/2026/20260503123556821.png)

## 0x05 绑定域名

Cloudflare 默认域名太长，建议绑定自己的域名。

> 你可以直接在 CF 中购买域名，或者如果你有域名的话，可以进行域名的绑定。

操作路径：
**项目 Settings → Domains and Routes → Add domain**

输入你的域名 → Add Domain → 按照提示解析即可。

绑定成功后效果：

![](https://raw.githubusercontent.com/HANDSOMEskuld/pics/main/2026/20260503125624172.png)

![697](https://raw.githubusercontent.com/HANDSOMEskuld/pics/main/2026/20260503125705011.png)

## 0x06 最后

用这个方法，**完全免费**就能拥有一个专业、美观、可持续运营的个人博客。

我的博客地址： https://prothistle.com

后续我也会把 𝕏 上的内容同步到博客，同时开通 Google AdSense，实现一份创作、两份收入。

**草友们冲就完事儿了！**

有任何问题欢迎在评论区留言，我看到都会回复。
