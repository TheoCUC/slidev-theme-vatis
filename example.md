---
theme: ./
contents:
  - Slidev简介
  - 主题介绍
  - 使用说明
  - 进度安排(占位符)
  - 进度安排(占位符)
  - 进度安排(占位符)
  - 进度安排(占位符)

---

# VATIS 非官方 Slidev 模板

中国传媒大学 视听技术与智能控制系统文化和旅游部重点实验室 非官方作品

---
layout: contents
---


---
layout: part
id: 1
---


---
id: 1
---


# Slidev

Slidev is a slides maker and presenter designed for developers, consist of the following features

- 📝 **Text-based** - focus on the content with Markdown, and then style them later
- 🎨 **Themable** - theme can be shared and used with npm packages
- 🧑‍💻 **Developer Friendly** - code highlighting, live coding with autocompletion
- 🤹 **Interactive** - embedding Vue components to enhance your expressions
- 🎥 **Recording** - built-in recording and camera view
- 📤 **Portable** - export into PDF, PNGs, or even a hostable SPA
- 🛠 **Hackable** - anything possible on a webpage

<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)

---
id: 1
---

# Navigation

Hover on the bottom-left corner to see the navigation's controls panel

## Keyboard Shortcuts

|     |     |
| --- | --- |
| <kbd>space</kbd> / <kbd>tab</kbd> / <kbd>right</kbd> | next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

---
layout: part
id: 2
---

---
id: 2
---

# 主题页面类型

该Slidev主题拥有以下几个板式：

* 封面
* 目录页
* 分章节页
* 正文页

这个Slider的目录、章节title、以及正文页上方的title都依赖于扉页中的 `contents` 内容， 如有需要，请按照 `yaml` 语法填写这一内容。

<scrool class="max-h-30">


## 封面

使用 **一级标题+正文** 书写即可。

## 目录页、分章节页

不需要填写内容，只需要指定 `layout` 为 `contents` 或 `part` 即可，对于分章节页，需要手动输入 `id`，**从1开始计数**。

## 正文页

正常书写即可，如需显示顶部title，在本页slider前标注本页的ID，注意**从1开始计数**。

</scrool>


---
id: 2
---

# 主题组件

## 滚动框

使用Slidev等前端技术做Slider的一个好处就是：可以突破传统PPT的版面限制，结合网页的形式进行展示交互。

如过长的图片、表格、文章等，在没有必要分页展示时，可以通过上下滚动来完整的展示。

滚动框效果如下，使用方法见README文档：

<scrool h=30>

|     |     |
| --- | --- |
| <kbd>space</kbd> / <kbd>tab</kbd> / <kbd>right</kbd> | next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

</scrool>

---
id: 2
---

# 主题组件

## 图片框

在使用Markdown制作Slider时，常遇到图片排版不够美观的问题。在Slidev中插入图片可以使用Markdown语法或HTML语法：
* `![Title](URL)`
* `<img src="URL">`

使用HTML语法虽然可以结合`WindiCSS`进行图片样式的调整，但实际上常在Slider中使用的图片布局无非就几种，因此增加了`<mimage>`标签，可以用于方便地插入图片，并在三种排版板式中切换。

* 水平居中，上下环绕式
* 向右浮动式
* 右上角悬浮式

---
id: 2
---

# 主题组件

## 图片框（水平居中，上下环绕式）


```
<mimage layout="c" url="https://cn.sli.dev/logo.svg" class="h-50" />
```

<mimage layout="c" url="https://cn.sli.dev/logo.svg" class="h-50" />

Slidev 旨在为开发者提供灵活性和交互性，通过使用他们已经熟悉的工具和技术，使他们的演示文稿更加有趣、更具表现力和吸引力。

---
id: 2
---

# 主题组件

## 图片框（向右浮动式）


```
<mimage layout="r" url="https://cn.sli.dev/logo.svg" class="h-50" />
```

<mimage layout="r" url="https://cn.sli.dev/logo.svg" class="h-50" />

Slidev 旨在为开发者提供灵活性和交互性，通过使用他们已经熟悉的工具和技术，使他们的演示文稿更加有趣、更具表现力和吸引力。

当使用所见即所得的编辑器时，人们很容易被样式选项所干扰。Slidev 通过分离内容和视觉效果来弥补这一点。这使你能够一次专注于一件事，同时也能够重复使用社区中的主题。Slidev 并不寻求完全取代其他幻灯片制作工具。相反，它专注于迎合开发者社区的需求。


---
id: 2
---

# 主题组件

## 图片框（右上角悬浮式）

Slidev 旨在为开发者提供灵活性和交互性

通过使用他们已经熟悉的工具和技术

使他们的演示文稿更加有趣、更具表现力和吸引力。

当使用所见即所得的编辑器时

人们很容易被样式选项所干扰. Slidev 通过分离内容和视觉效果来弥补这一点. 

**由于这个图片定位使用了Absolute，它会与文字部分重叠，建议只有在Slider左边只有短文字时使用**


<mimage layout="rt" url="https://cn.sli.dev/logo.svg" class="h-50" />

```
<mimage layout="rt" url="https://cn.sli.dev/logo.svg" class="h-50" />
```


---
id: 3
---

该主题是基于实验室Powerpoint模板制作的Slidev模板，适用于组会、简单的学术汇报等场景。

目前已知该主题会出现一些问题：
* 在Mac与iPad上的元素定位可能会不大一致
* 导出为pdf时，每页下方会有一条白线
* 导出为pdf时，最后一页下方会有一块白色区域，可以在最后插入空白页并删除pdf中的空白页解决

在HTML标签中使用Markdown内容时，要注意HTML标签与Markdown内容之间要有空行，否则不能正常解析。

在该主题中使用了许多图片资源，当全局安装Slidev、本主题使用时，会导致图片资源不能被正常解析。可以考虑将 `public` 文件夹下的图片拷贝到 `.md` 的 `public` 目录，或将图片资源上传到自己的图床，并修改模板中的链接。

欢迎大家使用并提出建议！