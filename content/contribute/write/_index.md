---
title: "如何为本站写文章"
date: 2021-01-29T22:00:25-05:00
draft: false
---

# 准备工作

## markdown

在开始之前，请找一份 markdown 的速查表花五分钟看一下。本文不再赘述。

比如说 [这篇](https://www.markdown.xyz/cheat-sheet/)

## 目录结构

如果您不满足于编辑已有的文章。而想创建新的文章，您应该先读一读这篇 [如何安排网站内容](../manage)。

# 如何引用本站内部的其它内容

我们推荐使用相对路径来引用本站中的其它内容。这样写起来简洁，而且在插入图片时，大部分 markdown 编辑器支持预览图片效果。

Hugo 可以自动解析和转换链接，所以只需要写清相对路径即可。对于本身独立成篇的 md 文件，相对路径很容易理解。对于`_index.md`，计算相对路径时应去掉`_index.md`，直接按其所属目录来计算，因为`_index.md`代表的就是这个目录。

另外，引用另一个 md 文件时，不需要写扩展名。

举例来说，本文在`content`目录中的路径是`contribute/write/_index.md`，如果我想引用上一级目录的文章，比如说`contribute/_index.md`，只需要写 `[请加入我们！](../)` 就可以了。而如果想引用 `contribute/why-hugo.md`，只需要写 `[使用 hugo 的理由](../why-hugo)` 就可以了。

上面两个例子的实际效果如下：

[请加入我们！](../)

[使用 hugo 的理由](../why-hugo)

# 如何插入图片

如果您已经读过了 markdown 速查表的话，应该知道插入图片就是用 `![文字说明](图片地址)` 的形式就可以了。

如果图片不在本站上，那么小括号中直接放图片的 URL 就可以。如果需要上传图片的话，您需要在 md 文件所属的目录里上传图片。然后就可以在小括号中直接填入图片文件名。本站的 GitHub 教程就是一个[例子](https://github.com/fuzhujishu/fuzhutech/blob/main/content/contribute/github/_index.md)。
