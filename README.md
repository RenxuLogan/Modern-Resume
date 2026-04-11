# 🚀 Modern Academic & Research CV Template 

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![LaTeX-XeLaTeX-Compatible](https://img.shields.io/badge/LaTeX-XeLaTeX-green.svg)](https://www.overleaf.com/)
[![Support-Chinese-English](https://img.shields.io/badge/Language-CN%2FEN-orange.svg)]()

一个专为学术申请及求职设计的 LaTeX 简历模板。其核心特色在于使用了 **TikZ 绘制的蓝色梯形标题栏**，在保持严谨学术风的同时，赋予了页面极具现代感的视觉张力。

---

## 📸 预览 (Preview)

<p align="center">
  <img src="image.png" alt="简历预览图" width="550px" style="max-width: 100%;">
</p>

---

## ✨ 核心特性 (Key Features)

- **💎 独创视觉设计**：采用 TikZ 矢量绘图定义的 Section 标题，自带蓝色梯形装饰与横向延伸线，层次感极强。
- **🌏 完美中英支持**：基于 `ctex` 宏包深度定制，完美解决中文字符渲染与字体对齐问题。
- **📑 结构化宏命令**：
  - `\resumeResearchHeading`：专门优化了科研/实习展示，支持“项目名称 + 身份/角色”的双向对齐排版。
  - `\resumeEducationHeading`：清晰展示教育背景及核心课程。
- **🛠️ 跨专业适用**：虽然初衷是为 CS 学生设计，但其**高信息密度**和**模块化**的排版同样适用于经管、法学、理工科等全学科。
- **📏 页面平衡优化**：预设了合理的垂直间距与边距设置，确保内容不满时依然视觉饱满，内容多时可自动适配。

---

## 🚀 快速上手 (Quick Start)

### 1. 环境要求
本模板必须使用 **XeLaTeX** 引擎进行编译，以确保中文字体正常显示。

### 2. 在 Overleaf 中使用
1. 新建项目并上传 `main.tex`。
2. 在左侧菜单 **Menu** -> **Compiler** 中选择 **XeLaTeX**。
3. 点击 **Recompile** 即可生成。

### 3. 本地编译
确保安装了完整的 TeX Live 或 MiKTeX 环境：
```bash
xelatex main.tex
````

-----

## 🎨 自定义指南 (Customization Guide)

本模板提供了极高的自由度，你可以通过修改 `main.tex` 顶部的参数轻松定制个人风格：

#### 1\. 颜色与视觉风格 (Theme Colors)

  * **更改主题色**：定位到 `\definecolor{MyDarkBlue}{RGB}{0, 50, 100}`。
      * 想要**学术深红**？尝试：`{139, 0, 0}`
      * 想要**高级纯黑**？尝试：`{0, 0, 0}`
  * **标题梯形宽度**：在 `\titleformat{\section}` 宏定义中，修改 `inner xsep=10pt` 即可调整标题文字左右的蓝色留白长度。

#### 2\. 页面布局与间距 (Layout & Spacing)

  * **整体边距**：修改 `\addtolength{\oddsidemargin}{-0.7in}` 系列参数。
      * **内容较多**：减小数值（如 `-0.8in`）以扩大书写区域。
      * **内容较少**：增大数值（如 `-0.5in`）使页面更聚拢，不显空旷。
  * **板块间距**：
      * **Section 间距**：修改 `\titlespacing*{\section}{0pt}{12pt}{6pt}`。`12pt` 为上方间距，`6pt` 为下方间距。
      * **列表缩进**：修改 `leftmargin=0.15in` 调整圆点列表距离左边界的缩进。
  * **微调行间距**：在列表环境中使用 `\vspace{-2pt}` 可细化每一项之间的紧凑度。

#### 3\. 字体与文字 (Fonts & Text)

  * **字间距**：姓名部分使用了 `\ziju{0.2}`。数值越大，中文名字越舒展，建议在 0.1 到 0.5 之间尝试。
  * **字体样式说明**：
      * `\textbf{...}`：加粗，建议用于机构名或奖项名。
      * `\textit{...}`：斜体，常用于日期或地理位置。
      * `\scshape`：小型大写字母，已应用于页眉姓名，彰显专业感。

#### 4\. 模块复用指令 (Command Reference)

模板预设了四种核心命令，方便一键调用：

  * `\resumeEducationHeading`：教育经历专用，左学校右时间。
  * `\resumeResearchHeading`：**科研/项目核心推荐**。左项目名右时间，支持在行内配合 `\hfill` 标注身份（如 `[第一作者]`）。
  * `\resumeItem`：标准圆点列表条目，自带微调间距。
  * `\resumeProjectHeading`：精简版项目/奖项条目，适用于单行展示。

-----

## 📜 许可 (License)

本仓库基于 **MIT License** 开源。你可以自由地使用、修改和分发，但请保留原作者的署名。

-----

## 🤝 贡献与反馈

如果你喜欢这个模版，欢迎点个 **Star** ⭐！如果你有更好的排版改进建议，欢迎提交 Pull Request 或通过 [Issues](https://github.com/RenxuLogan/Modern-Resume/issues) 反馈。
