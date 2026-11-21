---
layout: post
title: 学习 Markdown 写作技巧的示例文章
subtitle: 还有很多值得学习！
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [测试]
comments: true
mathjax: true
author: 比尔·史密斯
---

{: .box-success}
这是一篇演示文章，用来说明如何通过 Markdown 写博客。我很建议你[花 5 分钟学习 Markdown](https://markdowntutorial.com/)；它会教你把普通文本转换为粗体、斜体、表格等格式。<br/>也建议查看[生成本文的源代码](https://raw.githubusercontent.com/daattali/beautiful-jekyll/master/_posts/2020-02-28-sample-markdown.md)，学习在 Beautiful Jekyll 中使用 Markdown 的更多进阶技巧。

**这是一段粗体文字**

## 这是一个二级标题

[这是一个指向其他网站的链接](https://deanattali.com/)，[这是一个指向本文某个章节的链接](#项目站点中的本地链接)。

下面是一张表：

| 数字 | 下一个数字 | 上一个数字 |
| :------ |:--- | :--- |
| 五 | 六 | 四 |
| 十 | 十一 | 九 |
| 七 | 八 | 六 |
| 二 | 三 | 一 |

你可以使用 [MathJax](https://www.mathjax.org/) 编写 LaTeX 表达式。例如，当 \\(a \ne 0\\) 时，方程 \\(ax^2 + bx + c = 0\\) 有两个解：$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

来一份可丽饼怎么样？

![可丽饼](https://beautifuljekyll.com/assets/img/crepe.jpg)

它也可以居中显示！

![可丽饼](https://beautifuljekyll.com/assets/img/crepe.jpg){: .mx-auto.d-block :}

下面是一段代码：

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

下面是带语法高亮的相同代码：

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

下面是带行号的相同代码：

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## 提示框
你可以像下面这样添加通知、警告和错误提示框：

### 通知

{: .box-note}
**提示：** 这是一个通知提示框。

### 警告

{: .box-warning}
**警告：** 这是一个警告提示框。

### 错误

{: .box-error}
**错误：** 这是一个错误提示框。

## 项目站点中的本地链接 {#local-urls}

当你在 GitHub Pages 上托管*项目站点*（例如 `https://USERNAME.github.io/MyProject`）时，以 `/` 开头并指向本地文件的 URL 可能无法正常工作，因为 GitHub Pages 对根 URL（`/`）的解释有所不同。你可以在[常见问题](https://beautifuljekyll.com/faq/#links-in-project-page)中了解更多。为了演示这个问题，如果你的网站是项目站点，下面这张本地图片将无法显示：

![可丽饼](/assets/img/crepe.jpg)

如果上面的图片无法显示，请按[常见问题](https://beautifuljekyll.com/faq/#links-in-project-page)中的说明操作。下面是修复后的效果：

![可丽饼]({{ '/assets/img/crepe.jpg' | relative_url }})

<details markdown="1">
<summary>点击这里！</summary>
这里是一个**可展开**的章节。
</details>
