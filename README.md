<p align="center"><img src="assets/repository-cover.png" width="100%" alt="Cover Generator · 把文档做成封面"></p>

<h1 align="center">中文社交媒体封面生成器</h1>

<p align="center">把文案、文档或项目说明交给 Codex。选一种版式，配上你的照片，生成一张 3:4 竖版封面。</p>

<p align="center">
  <a href="#安装"><strong>安装到 Codex ↓</strong></a>　·　<a href="#六种模板">浏览模板画廊</a>　·　<a href="#使用方式">做第一张封面</a>
</p>

## 安装

**复制给你的 Agent**，让它完成全局安装和检查。

```text
请从 https://github.com/qiushibang/cover-generator 全局安装 cover-generator 到 Codex。
请检查 SKILL.md、references 和六张模板图片是否齐全，然后告诉我如何开始使用。
```

<details>
<summary>手动安装或下载 ZIP</summary>

```bash
git clone https://github.com/qiushibang/cover-generator.git ~/.codex/skills/cover-generator
```

也可以[下载安装包](https://github.com/qiushibang/cover-generator/raw/refs/heads/main/cover-generator.zip)，解压到 `~/.codex/skills/`。

</details>

## 六种模板

按你要讲的内容选版式。点击预览可看原图，生成时告诉 Codex 对应编号即可。

### 讲课程与方法

<table>
<tr>
<td width="50%" valign="top"><a href="assets/templates/01-classroom-checklist.png"><img src="assets/gallery/01-classroom-checklist.jpg" width="380" alt="课堂清单模板预览"></a><br><strong>01 · 课堂清单</strong><br>把课程收益拆成几条清单</td>
<td width="50%" valign="top"><a href="assets/templates/05-notebook-callouts.png"><img src="assets/gallery/05-notebook-callouts.jpg" width="380" alt="手账标注模板预览"></a><br><strong>05 · 手账标注</strong><br>用批注讲清一个方法</td>
</tr>
</table>

### 演示工具与产品

<table>
<tr>
<td width="50%" valign="top"><a href="assets/templates/03-light-tech-code-card.png"><img src="assets/gallery/03-light-tech-code-card.jpg" width="380" alt="技术步骤模板预览"></a><br><strong>03 · 技术步骤</strong><br>并排展示参数与操作步骤</td>
<td width="50%" valign="top"><a href="assets/templates/04-light-tech-product-card.png"><img src="assets/gallery/04-light-tech-product-card.jpg" width="380" alt="产品演示模板预览"></a><br><strong>04 · 产品演示</strong><br>给界面与工作流留出大幅画面</td>
</tr>
</table>

### 做短视频与创作教程

<table>
<tr>
<td width="50%" valign="top"><a href="assets/templates/02-dark-high-contrast.png"><img src="assets/gallery/02-dark-high-contrast.jpg" width="380" alt="暗底高对比模板预览"></a><br><strong>02 · 暗底高对比</strong><br>用大标题突出一个结论</td>
<td width="50%" valign="top"><a href="assets/templates/06-neon-self-media-board.png"><img src="assets/gallery/06-neon-self-media-board.jpg" width="380" alt="荧光信息板模板预览"></a><br><strong>06 · 荧光信息板</strong><br>把多个功能排成流程图</td>
</tr>
</table>

## 使用方式

安装后新开一次 Codex 对话，附上一张清晰的个人照片。下面以一份工具教程为例。

```text
用 $cover-generator 给我上传的工具教程做一张封面。
先展示六种模板给我选，再从文档里提炼标题和两个操作要点，用我附的照片排版。
```

| 你手头的素材 | 可以怎样告诉 Codex |
| :--- | :--- |
| 已写好的标题和要点 | “保留我的标题，把三个要点排成课堂清单。” |
| 课程讲义或产品文档 | “从附件里找出读者能学会的两件事，写到封面上。” |
| 当前项目目录 | “根据这个项目的 README，提炼一句用途和两个已实现的功能。” |

<details>
<summary>照片、内容来源与生成规则</summary>

六张模板采用合成插画。制作个人封面时，技能以你主动提供的照片作为人物参考。处理项目目录时，优先读取 README、项目文档和配置，并默认跳过密钥、缓存和构建产物。

[查看模板排版规则](references/template-guide.md) · [查看文案提炼规则](references/content-source-workflow.md)

</details>
