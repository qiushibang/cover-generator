<p align="center">
  <img src="assets/repository-cover.png" alt="Cover Generator repository cover" width="100%" />
</p>

# Cover Generator｜封面生成

一个面向中文社交媒体的 Codex 封面生成技能。它可以从手动文案、上传文档或当前项目目录中提炼内容，再结合用户个人照片和六种内置模板，生成具有斜向动势的 3:4 图文封面。

## 核心能力

- 生成前展示六种视觉模板，由用户明确选择。
- 支持手动文案、上传文档、当前工作目录三种内容来源。
- 自动提炼主题标签、两行标题、简短副标题和两至三个卡片要点。
- 使用用户本人照片，并尽量保持脸部、发型、服装和自然姿势。
- 统一使用倾斜背景、斜向标题和非方正展示字体，同时保留各模板的独立风格。
- 在完整尺寸和缩略图尺寸下检查中文文字、人物识别度与模板一致性。

## 六种模板

<table>
  <tr>
    <td align="center"><img src="assets/templates/01-classroom-checklist.png" width="220" /><br/><b>01 课堂清单</b></td>
    <td align="center"><img src="assets/templates/02-dark-high-contrast.png" width="220" /><br/><b>02 暗底高对比</b></td>
    <td align="center"><img src="assets/templates/03-light-tech-code-card.png" width="220" /><br/><b>03 浅色技术卡片</b></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/templates/04-light-tech-product-card.png" width="220" /><br/><b>04 产品演示卡片</b></td>
    <td align="center"><img src="assets/templates/05-notebook-callouts.png" width="220" /><br/><b>05 手账标注</b></td>
    <td align="center"><img src="assets/templates/06-neon-self-media-board.png" width="220" /><br/><b>06 荧光信息板</b></td>
  </tr>
</table>

六张内置模板均为重新绘制的合成示意图，不含真人照片、可识别人脸或第三方品牌标志。模板图片只用于构图与风格参考；只有在生成最终封面时，才使用用户主动提供并授权处理的个人照片。生成结果不得复制模板文字、账号标识、水印或未经授权的品牌标志。

## 安装

将仓库直接克隆到 Codex 全局技能目录：

```bash
git clone https://github.com/qiushibang/cover-generator.git ~/.codex/skills/cover-generator
```

也可以下载仓库中的 `cover-generator.zip`，解压到 `~/.codex/skills/`。

## 使用方式

安装后新建一次对话，并描述需要制作中文社交媒体封面。技能会依次：

1. 展示全部六种模板。
2. 让用户选择模板，并收集个人照片。
3. 从手动文案、上传文档或当前目录中获得内容。
4. 自动生成封面文案并制作图片。
5. 检查文字准确性、人物识别度和斜向视觉效果。

示例：

```text
请使用 Cover Generator，根据我上传的项目说明和个人照片制作封面。
```

## 目录结构

```text
cover-generator/
├── SKILL.md
├── README.md
├── assets/
│   ├── repository-cover.png
│   └── templates/
└── references/
    ├── content-source-workflow.md
    └── template-guide.md
```

## 内容与隐私边界

读取当前工作目录时，技能优先使用 README、项目文档和项目配置；默认排除环境变量、密钥、令牌、依赖目录、构建产物、缓存与数据库导出。封面文案必须来自可核验的输入内容，不得虚构效果、指标或产品能力。
