# 个人学习博客

这是一个使用 [Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll) 主题搭建的个人博客，部署在 GitHub Pages。

## 技术

- **Jekyll**：生成静态网站
- **Markdown**：编写博客文章
- **MathJax 3**：渲染 LaTeX 数学公式，支持 `$...$` 行内公式和 `$$...$$` 块级公式
- **不蒜子**：统计并在文章页显示浏览次数

## 补充与调整

- 将网站页面、导航和界面文案改为中文
- 增加学习笔记分类，并整理大语言模型相关笔记
- 调整 MathJax 配置以支持常见的行内公式写法
- 在文章模板中加入按页面统计的浏览次数
- 使用 `待发布/` 保存尚未完成的笔记，并通过 `.gitignore` 排除该目录

文章放在 `_posts/` 中，图片放在 `assets/img/` 中。文章需要包含 Jekyll YAML Front Matter；数学公式文章需设置 `mathjax: true`。
