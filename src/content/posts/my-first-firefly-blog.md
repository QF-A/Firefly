---
# ============================================
# 文章Front Matter配置（必须放在文件开头，用---包裹）
# ============================================

# 文章标题（必填，显示在文章列表和详情页）
title: "我的第一篇学习笔记：Firefly博客搭建"

# 文章发布日期（必填，格式：YYYY-MM-DD）
published: 2026-05-09

# 文章更新日期（可选，不填则使用发布日期）
updated: 2026-05-09

# 是否将此文章置顶在文章列表顶部
pinned: false

# 文章标签（可选，数组格式，用于分类和搜索）
tags: ["学习笔记", "Firefly", "博客搭建", "Astro"]

# 文章分类（可选，单分类）
category: "技术学习"
  
# 文章封面图片路径
image: "./ChatGPT Image 2026年5月16日 22_08_58.png"

# 文章的简短描述，显示在首页上
description: "我在Firefly的第一篇博客，记录了我从零开始搭建Firefly个人博客的完整过程，包括环境安装、源码拉取、配置修改和文章发布等。"

# 是否为草稿（可选，true=隐藏，false=显示）
draft: false

# 文章作者
author: "清风不是F."

# 文章URL路径（可选，不填则使用文件名作为URL）
slug: "hello-firefly"
---

  
<!-- ![alt text](<ChatGPT Image 2026年5月16日 22_08_58.png>) -->
# 我的第一篇学习笔记

## 前言

这是我用Firefly搭建的个人博客的第一篇文章。我是希望通过这个博客记录我的学习成长历程，分享我的技术经验。  

## 为什么选择Firefly

我选择Firefly作为我的博客框架，主要有以下几个原因：

1. **颜值高**：开箱即有现代化的UI设计和精美的动画效果，比传统的Hexo主题好看太多

2. **技术栈新**：基于Astro+Tailwind CSS+TypeScript，都是2026年前端和AI Web开发的主流技术

3. **易于使用**：配置简单，Markdown写作体验好，不需要复杂的前端知识

4. **性能优秀**：静态站点生成，首屏加载速度极快，Lighthouse评分95+

5. **部署方便**：支持Cloudflare Pages一键部署，国内访问速度快，完全免费


## 搭建过程

### 1. 环境准备

首先安装Git、Node.js ≥22、pnpm ≥9和VS Code，这是Firefly运行的基础环境。
 - [Git](https://git-scm.com/install/windows)：版本控制工具，用于管理项目源码
 - [Node.js](https://nodejs.org/zh-cn)：JavaScript运行环境，用于运行项目脚本
 - pnpm：包管理工具，用于安装依赖，终端执行：`npm install -g pnpm`
 - [VS Code](https://code.visualstudio.com/)：代码编辑器，用于编写和调试项目代码，用于修改配置、写文章


  
### 2. 源码托管 | Fork Firefly官方仓库

#### 一、前言
通过Fork官方仓库(https://github.com/CuteLeaf/Firefly)，获取自己的独立仓库，可自由修改配置、增删内容、同步官方更新，之后推送代码到该仓库，Cloudflare会自动触发构建部署。

#### 二、Fork操作

1. 打开[Firefly仓库](https://github.com/CuteLeaf/Firefly)，点击右上角的 Fork 按钮(先要登录GitHub)，创建自己的仓库。
**关键说明：** Fork后的仓库归你所有，修改内容不会影响官方仓库，后续可一键同步官方更新，适合长期维护
2. 进入刚刚创建的仓库，点击 Code 按钮，复制仓库地址
3. 在终端中，进入你的本地项目目录，执行以下命令：`git clone https://github.com/你的用户名/Firefly.git`
4. 进入项目目录：`cd Firefly`命令

### 3. 本地依赖安装与启动（仅用于本地预览）

1. 执行`pnpm install`命令安装了所有项目依赖。
2. 运行`pnpm dev`命令启动本地开发服务器
3. 等待10~30秒，终端显示访问地址：`http://localhost:4321`
4. 打开浏览器，访问地址：`http://localhost:4321`，看到Firefly默认首页，则本地搭建成功！
5. 停止服务：`Ctrl+C`

### 5. 配置修改

在VSCode中修改了`siteConfig.ts`，`profileConfig.ts`文件，配置了网站标题、作者信息。
  
### 6. 文章创作

创建了这篇Markdown文章，记录我的搭建过程。

## 学习感悟

通过这次博客搭建，我不仅拥有了一个属于自己的技术博客，还学习到了 Git、Node.js、pnpm 等工具的使用方法。更重要的是，我接触到了 Astro 这个现代静态站点生成器，这对我未来的 AI Web 开发学习有很大的帮助。

  

## 后续计划

- 持续更新学习笔记，记录我的技术成长历程

- 美化博客主题，添加更多个性化元素

- 配置 Twikoo 评论系统，方便与读者交流

- 学习 Astro 框架，开发自己的博客功能

  

## 总结

搭建个人博客是技术学习的重要一步，它不仅可以帮助我们记录学习过程，沉淀知识体系，还可以展示我们的技术能力，建立个人品牌。希望我能坚持写博客，不断提升自己的技术水平。