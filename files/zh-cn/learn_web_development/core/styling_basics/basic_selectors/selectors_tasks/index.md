---
title: 技能测试：选择器
slug: Learn_web_development/Core/Styling_basics/Basic_selectors/Selectors_Tasks
original_slug: Learn/CSS/Building_blocks/Selectors/Selectors_Tasks
---

{{LearnSidebar}}

这个任务的目的是帮助你理解 CSS 里的选择器。

> [!NOTE]
> 你可以在下面的交互式编辑器中尝试解决问题，然而把代码下载然后使用一个在线工具比如 [CodePen](https://codepen.io/)、[jsFiddle](https://jsfiddle.net/) 或 [Glitch](https://glitch.com/) 去解决这些问题可能对你更有作用。
>
> 如果你卡住了，可以向我们寻求帮助——请参阅本页底部的[打分评估或进一步帮助](#打分评估或进一步帮助)部分。

## 任务一

在此任务中，请在不改变 HTML 的情况下，使用 CSS 去完成下面的要求：:

- 使`<h1>`的字体颜色为蓝色
- 使`<h2>`有一个蓝色背景且白色文本。
- 使`<span>`中的文本的字体大小为 200%。

你的结果应该看起来和下面这张图一样：

![Text with the CSS applied for the solution to task 1.](selectors1.jpg)

尝试更新下面的实时代码，以重现完整的示例：

{{EmbedGHLiveSample("css-examples/learn/tasks/selectors/type.html", '100%', 700)}}

<details>
<summary>点击显示答案</summary>

You need to target the `h1`, `h2` and `span` selectors to change their color or size.

```css
h1 {
  color: blue;
}

h2 {
  background-color: blue;
  color: white;
}

span {
  font-size: 200%;
}
```

</details>

> [!CALLOUT]
>
> 如需提交测评或进一步练习，[下载本任务的初始文件](https://github.com/mdn/css-examples/blob/main/learn/tasks/selectors/type-download.html)，然后在本地或在线编辑器中练习。

## 任务二

在此任务中，我们希望你在不改变 HTML 的情况下，对本例中内容的外观进行以下更改：

- 让 id 为 `special` 的元素有一个黄色背景。
- 让类为 `alert` 的元素有一个 2px 的灰色边框。
- 如果一个元素同时为 `alert` 类和 `stop`类，让它的背景变为红色。
- 如果一个元素同时为 `alert` 类和 `go`类，让它的背景变为绿色。

你的结果应该看起来和下面这张图一样：

![Text with the CSS applied for the solution to task 2.](selectors2.jpg)

尝试更新下面的实时代码，以重现完整的示例：

{{EmbedGHLiveSample("css-examples/learn/tasks/selectors/class-id.html", '100%', 800)}}

<details>
<summary>点击显示答案</summary>

这个任务测试你是否理解了类选择器和id选择器之间的区别，以及如何选择同时具有多个类的元素。

```css
#special {
  background-color: yellow;
}

.alert {
  border: 2px solid grey;
}

.alert.stop {
  background-color: red;
}

.alert.go {
  background-color: green;
}
```

</details>

> [!CALLOUT]
>
> 如需提交测评或进一步练习，[下载本任务的初始文件](https://github.com/mdn/css-examples/blob/main/learn/tasks/selectors/class-id-download.html)，然后在本地或在线编辑器中练习。

## 任务三

在此任务中，请尝试在不添加 HTML 的情况下进行以下更改。

- 为链接添加样式，使得链接为橘色，被访问后变为绿色，在鼠标悬停状态下移除链接文本的下划线。
- 为容器里的第一个元素设置`font-size: 150%`，并且将这个元素的第一行变为红色。
- 通过选择表格中每隔一行的行，并将其背景色设为 `#333`，前景色设为白色，来实现表格隔行变色。

你的结果应该看起来和下面这张图一样：

![Text with the CSS applied for the solution to task 3.](selectors3.jpg)

尝试更新下面的实时代码，以重现完整的示例：

{{EmbedGHLiveSample("css-examples/learn/tasks/selectors/pseudo.html", '100%', 800)}}

<details>
<summary>点击显示答案</summary>

使用伪类 (`:first-child`) 和伪元素 (`::first-line`)。
设置 `a` 元素的 `:link`、`:visited` 和 `:hover` 状态的样式，并使用 `:nth-child` 伪类创建条纹表格行。

```css
.container p:first-child {
  font-size: 150%;
}

.container p:first-child::first-line {
  color: red;
}

a:link {
  color: orange;
}

a:visited {
  color: green;
}

a:hover {
  text-decoration: none;
}

tr:nth-child(even) {
  background-color: #333;
  color: #fff;
}
```
</details>

> [!CALLOUT]
>
> 如需提交测评或进一步练习，[下载本任务的初始文件](https://github.com/mdn/css-examples/blob/main/learn/tasks/selectors/pseudo-download.html)，然后在本地或在线编辑器中练习。

## 任务四

在此任务中，我们希望你：

- 将紧接在 `<h2>` 元素之后的段落文字颜色设为红色。
- 移除 `list` 类无序列表的直接子元素的列表项符号，并为其添加 1px 灰色下边框。

你的结果应该看起来和下面这张图一样：

![Text with the CSS applied for the solution to task 4.](selectors4.jpg)

尝试更新下面的实时代码，以重现完整的示例：

{{EmbedGHLiveSample("css-examples/learn/tasks/selectors/combinators.html", '100%', 800)}}

<details>
<summary>点击显示答案</summary>

这个任务旨在检查你是否理解如何使用不同的关系选择器。
以下是一个合适的解决方案：

```css
h2 + p {
  color: red;
}

.list > li {
  list-style: none;
  border-bottom: 1px solid #ccc;
}
```

</details>

> [!CALLOUT]
>
> 如需提交测评或进一步练习，[下载本任务的初始文件](https://github.com/mdn/css-examples/blob/main/learn/tasks/selectors/combinators-download.html)，然后在本地或在线编辑器中练习。

## 任务五

在此任务中，使用属性选择器添加 CSS 以实现：

- 选择带有 `title` 属性的 `<a>` 元素，将其边框颜色设置为粉色（`border-color: pink`）。
- 选择带有 `href` 属性且属性值中包含 `contact` 的 `<a>` 元素，将其边框颜色设置为橙色（`border-color: orange`）。
- 选择 `href` 属性值以 `https` 开头的 `<a>` 元素，将其边框颜色设置为绿色（`border-color: green`）。

你的结果应该看起来和下面这张图一样：

![Four links with different color borders.](selectors-attribute.png)

尝试更新下面的实时代码，以重现完整的示例：

{{EmbedGHLiveSample("css-examples/learn/tasks/selectors/attribute-links.html", '100%', 800)}}

<details>
<summary>点击显示答案</summary>

- 要选择带有 title 属性的元素，我们可以在方括号中添加 title（`a[title]`），这样会选中第二个链接，因为它是唯一带有 title 属性的链接。

- 选择 href 属性中包含 "contact" 的 <a> 元素，并将其边框设为橙色（border-color: orange）。
  这里需要匹配两种情况：`/contact` 和 `../contact`。因此，我们可以使用 `*=` 来匹配 href 值中任意位置包含 "contact" 的链接。这样会选中第三个和第四个链接。
  
- 选择 href 值以 https 开头的 <a> 元素，并将其边框设为绿色（border-color: green）。
  查找 `href` 值以 "https" 开头的链接，因此使用 `^=` 来仅选中第一个链接。

```css
a[title] {
  border-color: pink;
}
a[href*="contact"] {
  border-color: orange;
}
a[href^="https"] {
  border-color: green;
}
```

</details>

> [!CALLOUT]
>
> 如需提交测评或进一步练习，[下载本任务的初始文件](https://github.com/mdn/css-examples/blob/main/learn/tasks/selectors/attribute-links-download.html)，然后在本地或在线编辑器中练习。

## 打分评估或进一步帮助

你可以在上面的交互式编辑器中练习示例这些示例。

如果你想得到任务评价，或者遇到了问题需要帮助，请按如下操作进行：

1. 将你的作业上传到可共享的在线编辑器上，比如 [CodePen](https://codepen.io/)、[jsFiddle](https://jsfiddle.net/) 或 [Glitch](https://glitch.com/)。你可以自己编写代码，也可以使用上面给出的初始文件。
2. 在 [MDN 论坛的学习板块](https://discourse.mozilla.org/c/mdn/learn)上发帖以寻求打分或帮助。你的帖子中应包含：

   - 一个简述问题的标题。如“Assessment wanted for Selectors skill test 1”（请使用英文发帖）。
   - 详细描述你的尝试和你预期的网页效果。比如你在哪个位置需要帮助，或者你需要打分评估。
   - 你需要打分或帮助的作业链接（通过上述的在线编辑器上传）。只有让别人看到你的代码，你才能得到更好的帮助。
   - 本题的链接。让别人知道你所问的具体题目。
