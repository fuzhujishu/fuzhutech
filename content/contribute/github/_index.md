---
title: "如何使用 GitHub 编辑本站内容"
date: 2021-01-29T18:58:34-05:00
draft: false
---

# 开始之前

在动手开始编辑之前，请确保：

- 您有一个 GitHub 帐户。您可以在 [这里注册](https://github.com/join)

# 如何直接编辑文章

如果您已经联系过我们，并且我们已经给了您直接编辑本站文章的权限，那么您可以直接在浏览器中编辑文章。

在每一篇文章（包括这篇）的右上角，都有一个“Edit this page”的链接，点击这个链接，就可以跳转到相应的 GitHub 页面，然后点击垃圾桶图标左边的笔状图标即可修改文章。

![GitHub 文章预览页面右上角的按钮](github_edit.png)

# 如何在自己的仓库中编辑文章

首先，您需要创造我们站点的一个 fork。GitHub 官方对此有详尽的 [文档](https://docs.github.com/cn/github/collaborating-with-issues-and-pull-requests/working-with-forks)，但中文文档未免有些晦涩，因此我们在这里写一个简单的教程。

## 创建 fork （复刻）

首先访问[本站的 GitHub 仓库](https://github.com/xuan-w/fuzhutech)，然后点击页面右上角的 fork 按钮。

![GitHub 仓库页面右上角的按钮](github_fork.png)

点击之后按提示确认即可。

## 编辑文章

类似于 [直接编辑](#如何直接编辑文章)，您同样使用文章预览右上角的编辑按钮进行编辑。但您可能会不清楚如何找到您想编辑的文章的位置。

这很简单，比如说您直接点击浏览器中“Edit this page”得到如下示例链接

`https://github.com/fuzhujishu/fuzhutech/blob/main/content/contribute/github/_index.md`

您只需要编辑一下这个链接，将链接中的 fuzhujishu 替换为您自己的 GitHub 用户名就可以了。

特别需要注意的是，如果您不是第一次编辑文章，在您开始编辑之前，请确定您已经更新您的仓库到最新版本。具体请见 [如何重新 fork](#如何重新-fork)。

## 发 Pull Request

编辑完成之后，下一步是给我们发 Pull Request 以便我们可以审核您的编辑，并修正一些可能影响网站的问题。

在您仓库的主页，点击右上角的 Pull Request 按钮，按提示确认，即可发送 Pull Reqest。我们收到之后会及时将您的编辑合并到我们的文章中。

![GitHub 仓库内容右上角的按钮](github_PR.png)

## 如何重新 fork

如果您以前 fork 过我们的网站，但中间我们的网站又更新了，您在重新编辑之前，需要保持和我们的仓库同步。很遗憾的是，这个操作略有点麻烦。

有两种办法实现这个目标。第一个办法是删除仓库，重新 fork。第二种办法是 pull 我们的最新更改。后者也许改日可以发一个教程。现在我们先讲第一个办法。

1. 您首先需要备份好您原来仓库里的所有东西。
2. 在您仓库首页点右上角齿轮 Setting 按钮
3. 一路滚到页面最底下，点击“Delete this repository”
4. 重新[创建 fork](#创建-fork-复刻)
