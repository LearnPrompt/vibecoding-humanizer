# Carl UI Humanizer

面向两类任务：减少界面模板感，以及通过字体、构图、配色、材质、动效与参考转译提升审美。不是把所有页面改成极简，也不把加特效等同于好设计。

结构参照 [blader/humanizer](https://github.com/blader/humanizer)：工作方式、按类编号的识别条目、修改前后示例、保留条件和输出模式。UI内容重新整理自本次材料；不是原仓库的中文翻译，也不使用它的验证数据。

## 一个例子

**修改前**：页面名是素材库，副标题再解释这里可以管理素材。上传按钮旁又写点击上传。四个相关统计各用强阴影卡，卡片内继续套彩边框。

**修改后**：保留素材库、上传素材与真实格式／容量限制；相关统计合在一个分区。用对齐和间距表达关系，必要的表单标签、帮助、错误与状态继续可见。

这是规则说明示例，不是已在DeepSeek/Codex上完成的对照实测。

## 包含什么

```text
carl-ui-humanizer/
├── SKILL.md                     # 两种入口、八维设计流程与13条诊断
├── README.md
├── VALIDATION.md
├── agents/openai.yaml
├── references/
│   ├── prompt-library.md        # 14条可直接使用的编辑提示语
│   ├── aesthetic-reference.md   # 风格/动效原词与中文、参考选择
│   ├── english-originals-zh.md  # 原有英文原句与中文对应
│   ├── anthropic-prompts-en-zh.md # MIT官方前端审美完整英中提示
│   ├── expanded-sources.md      # 新增原句、原文入口与中文摘要
│   ├── source-coverage.md       # 来源核读范围及未完成部分
│   ├── original-materials.md    # 原始来源与编辑边界
│   └── code-animation.md
└── assets/source-luinlee.png
```

主入口先区分“去味”和“审美提升”。保留13条诊断，新增八维正向设计流程；[提示语库](references/prompt-library.md)完整保留用户确认的六条，再补参考转译、构图、材质、动效规格、响应式与验收。

[中英文词表](references/aesthetic-reference.md)可直接用于选择风格与描述动作。原文、忠实翻译、摘要、编辑适配分别标明；中文来源不会反译为假英文原文。明确有MIT许可的[Anthropic前端审美提示](references/anthropic-prompts-en-zh.md)保留完整英文、中文翻译及许可证；其他未确认许可的长篇第三方提示保留原文入口、短摘录和中文摘要。

## 怎么用

把完整文件夹交给支持Skills的Agent，或直接让Agent读取其中的SKILL.md。安装到宿主的Skill目录后可用 `$carl-ui-humanizer`；不同宿主是否能自动发现，需在该宿主确认。本仓库是独立 Skill 包，不包含插件市场注册或跨端同步。

### 给其他 Agent 的安装指令

复制下面这段给 Agent：

> 从 https://github.com/LearnPrompt/carl-ui-humanizer 安装 carl-ui-humanizer。先确认你当前宿主的 Skill 目录，将完整仓库放进该目录的 carl-ui-humanizer 子目录，保留 references、assets 和 agents。若同名目录已经存在，先检查，不要覆盖已有修改。安装后读取 SKILL.md，确认名称与版本，并报告宿主是否已识别；必要时提示我重开会话。

### Git 安装

目标目录必须不存在；以下命令不会自动覆盖已有安装。

```bash
# Codex：默认用户级目录；自定义 CODEX_HOME 时沿用该配置
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
git clone https://github.com/LearnPrompt/carl-ui-humanizer.git "${CODEX_HOME:-$HOME/.codex}/skills/carl-ui-humanizer"

# Claude Code：用户级目录（二选一，按宿主安装）
mkdir -p "$HOME/.claude/skills"
git clone https://github.com/LearnPrompt/carl-ui-humanizer.git "$HOME/.claude/skills/carl-ui-humanizer"
```

其他宿主请使用其实际 Skill 目录。也可下载仓库 ZIP，解压后将完整目录命名为 `carl-ui-humanizer`。不支持自动发现的 Agent 可以直接读取 `SKILL.md` 使用。主规则为中文，引用材料包含英文原文与中文对照，并非两套独立语言版 Skill。

示例请求：

> 使用这个包的SKILL.md检查素材管理页面，优先修影响理解和操作的问题；保留品牌、业务数据、必要帮助与现有功能，改完告诉我实际验证了什么。

也可以只给截图要求审查，或要求输出能复制给模型的修改指令。仅给截图时，不宣称按钮、接口或窄屏已经验证。

## 材料怎样重新提取

- 用户截图里的英文指令、线程中的英文补充与忠实中文翻译单独保留。
- 英文八维检查键逐项对应中文，循环与获奖目标另作解释。
- ZaynHao十条及Invo补充原来就是中文，按中文原帖提取。
- 网站清单、艺术风格和视频库是参考材料，后来八条文章指令是编辑适配，不混称英文翻译。

完整材料见 [原始素材与翻译边界](references/original-materials.md)。截图是用户提供的来源材料，不是改后UI效果图。

## 边界

不把所有卡片、渐变和英文小标题当错误；不强制0.5px边框、12px小字、全站Radix或所有动效250ms；不把UI规则直接套成动画叙事规则。没有明确问题时可以保留原设计。

本包直接支撑现有UI去AI味图文及后续页面改稿，采用现有素材与离线文档，不增加检测服务、自动评分、联网SDK或长期自动化。

## 结构参考快照

读取日期2026-10-28；参考仓库元数据版本3.1.0；修订 `8c307f367c91bd974002f10f2be2965d642c13df`。
[对应SKILL.md](https://github.com/blader/humanizer/blob/8c307f367c91bd974002f10f2be2965d642c13df/SKILL.md)

本包独立版本0.2.0。目录/frontmatter校验与离线行为演练的结果见 [验证记录](VALIDATION.md)；这不等同真实浏览器视觉、DeepSeek执行效果或线上部署验收。

## 0.2.0 来源补齐与覆盖范围

2026-11-05重查当前清单、收件箱及已完成历史，并重新核读可取得的正文、原图、视频采样和原始提示文件。具体状态见[来源覆盖与缺口](references/source-coverage.md)。已获取的收藏清单、已读原文/图片和实测效果分别记录；**不声称所有原帖和媒体均已读全**。

原有[英文原句与中文对照](references/english-originals-zh.md)保留，包括截图原句、线程补充与八维技术指令；新增来源见[扩展核读](references/expanded-sources.md)。未取得的原文不由模型猜补。
