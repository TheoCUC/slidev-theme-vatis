---
theme: ./
contents:
  - Slidev简介
  - 主题说明
  - 进度安排(占位符)
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

$$
  \int f(x) \, \rm d x \\
  \int f(x) \, \text{d} x
$$

<br>
<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)


---
id: 2
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

# 主题样式结构

如你所见，这个主题拥有「封面」、「目录页」、「Part页/分隔页」、「正文」这些丰富的样式. 

其中的目录页、分隔页以及正文只需要填入对应在目录里的序号（从1开始，如果大于10可能会有问题）就能正确显示对应的目录信息.

首先要在扉页中填入目录信息：

```
---
theme: ./
contents:
  - Slidev简介
  - 主题说明
  - 进度安排(占位符)
  - 进度安排(占位符)
  - 进度安排(占位符)
  - 进度安排(占位符)
  - 进度安排(占位符)

---
```

---
id: 2
---

# 主题样式结构

## 封面

对于封面，使用一级标题+正文来写

```
# VATIS 非官方 Slidev 模板

中国传媒大学 视听技术与智能控制系统文化和旅游部重点实验室 非官方作品
```

<br>
<br>

## 目录

目录页是自动生成的

```
---
layout: contents
---
```

---
id: 2
---

# 主题样式结构

## 分隔页

分隔页需要手动指定哪一个块 同样id从1开始


```
---
layout: part
id: 1
---


---
```

## 正文

至于正文，也是需要指定id来显示头顶的内容。其中的一级标题会被显示为左上角的小标签。

```
---
id: 1
---

# 主题样式结构
```

---
layout: part
id: 5
---


---
id: 1
---

# 123

```
---
layout: part
id: 5
---

---
id: 5
---
```

一定要注意 id 后面有个空格






