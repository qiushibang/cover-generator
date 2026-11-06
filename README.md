<p align="center"><img src="assets/repository-cover.png" width="100%" alt="cover-generator，展示高对比、产品卡片和手账三种内置版式"></p>

<h1 align="center">cover-generator</h1>

<p align="center"><strong>把课程讲义、项目说明或创作脚本，做成一张 3:4 图文封面。</strong><br>
A cover design skill for courses, projects and creators.</p>

<p align="center"><a href="#六种模板"><strong>浏览六种版式</strong></a>　·　<a href="#安装">复制安装指令</a>　·　<a href="#使用方式">制作第一张封面</a></p>

## 你想为哪份内容做封面？

| 准备发布 | 交给 Codex | 适合的版式 |
| :--- | :--- | :--- |
| 一期视频或专栏 | 脚本里最想让读者记住的观点 | **02 暗底高对比**，用一个大标题抓住重点 |
| 一堂课或一场分享 | 讲义、讲者照片，以及听众能学到什么 | **01 课堂清单**，把学习要点排在人物旁边 |
| 一个项目或产品 | 项目目录中的 README，或一份产品介绍 | **04 产品演示**，给功能说明留下完整的卡片区域 |

每次制作都用你提供的照片。六张内置参考图决定版式与配色，封面文字取自你的材料；需要换一种语言时，在请求里写明即可。

## 安装

在 Codex 中使用 `$cover-generator` 调用。把下面这段话复制给 Agent 即可安装。

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

点击图片可查看原尺寸模板。调用技能时，Codex 会先展示全部六张，让你选定编号再生成。

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

安装后新开一次 Codex 对话，附上一张清晰的个人照片和内容素材。例如，要给一场工作坊做封面，可以这样说。

```text
用 $cover-generator 给这场工作坊做一张竖版封面。附件是活动简介和我的讲者照片。
先展示六种模板给我选，再从简介里提炼标题和两个学习要点。这次请用西班牙语。
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
