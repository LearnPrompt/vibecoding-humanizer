# 验证范围

## 0.1.1 原包（2026-10-28）

- Skill Creator quick_validate、13条编号、内部相对链接和Agent元数据检查通过。
- 合成素材管理HTML离线改稿保留上传类型、容量限制、表单标签、状态与原JavaScript；并非真实产品验收。
- 原ZIP的7个文件及传到Mini的副本逐项核验一致。

## GitHub 分发整理（2026-11-04）

- 保留原包的 SKILL.md、agents、references 和来源截图，补充仓库安装说明及本记录。
- 不增加执行脚本、依赖、网络服务或自动更新机制。
- 发布前重新检查包结构、相对链接及与原包核心文件的一致性；发布后从GitHub重新克隆核验。

## 尚未验证

真实浏览器视觉与交互、窄屏与焦点实际体验、各宿主自动识别、DeepSeek或其他模型的对照效果。本仓库可分发，不代表上述验收已经完成。

## 0.2.0 来源补齐与行为检查（2026-11-05）

- 滴答只读扫描36个清单、收件箱和已完成历史分页，合并5530个唯一任务；检索196个关键词候选并补查相关目录子任务。没有修改滴答任务、归档或制作状态。
- 从原始正文、图片、原视频采帧与官方提示文件复核来源。当前在线读取与10/26、11/01保存后重新核读的证据分别标注；受阻与附件缺失见来源覆盖表。
- Anthropic三段英文与固定版本官方notebook字符串逐字比对一致，保留MIT版权许可。中文对照人工核读；其他长篇未授权来源使用短摘录、摘要和原文入口。
- 独立Agent前向检查三个请求：咖啡品牌审美方案、品牌指定Inter且不增依赖的报销系统去味、原文与翻译区分。均能保持任务约束；未发现阻断性行为问题。
- 独立事实复核发现并修正历史视频读取状态、S7风格迁移范围与MotionSites八类术语遗漏。测试发现的旧进度占位已替换为最终核读状态或明确缺口。
- Skill结构、Markdown本地引用、发布内容中的私有路径/访问令牌模式、元数据及Git空白检查通过。

本轮行为检查是阅读Skill后的方案输出，不是产品页面改造、浏览器交互验收或各Agent自动发现验收。没有使用模型或网站营销声称替代实际效果验证。新版增加可读材料与执行能力，但不声称所有收藏外链和图片均已读全。

## 0.3.0 改名 vibecoding-humanizer 与四模式路由（2026-11-05）

改动：Skill 名 `carl-ui-humanizer` → `vibecoding-humanizer`；SKILL.md 改为模式路由（3d / svg / html / ui + 混合规则 + 共用规则）；原八维流程与 13 条 UI 诊断原样移到 `references/mode-ui.md`；新增 `mode-3d.md`、`mode-svg.md`、`mode-html.md`；新增 `examples/` 前后效果（15 张从实测录屏/截图裁切压缩的 JPEG，共约 0.8 MB）；README 改为中英双语、npx 安装置顶；`agents/openai.yaml` 更新名称与默认提示。

### 静态检查（已做）

- frontmatter `name: vibecoding-humanizer`、`version: "0.3.0"`；全部 Markdown 本地链接 0 处断链；15 张示例图 ffprobe 可解码。
- 有效文档里旧名只出现在迁移说明、frontmatter「前身为」和 UI 案例的历史日志引用中。
- 发布内容扫描无本机路径（`/Users/`）、访问令牌模式；示例截帧已裁掉浏览器地址栏与无关对话面板。
- 动态海报含第三方照片（新京报、浦峰摄影等），再分发权限不确定，未收录；鹈鹕 SVG 只作成果展示，不当海报前版。

### 安装实测（已做，本地路径）

- 环境：macOS，Node v25.6.0，Skills CLI `skills@1.7.6`，`DISABLE_TELEMETRY=1`，临时 HOME 与临时项目目录。
- `npx skills add <本地仓库> -l` 识别到 1 个 Skill：vibecoding-humanizer。
- `npx skills add <本地仓库> --skill vibecoding-humanizer -a claude-code -y --copy` 安装到 `./.claude/skills/vibecoding-humanizer`，SKILL.md、5 个 mode/代码动画参考、其余 references、agents、examples 全部到位，与仓库逐文件一致。
- 远端命令见下一节「远端安装实测」。

### 远端安装实测（已做，2026-11-05，main = `b1f9dc1`）

- 同上环境，空 HOME、空项目目录。
- `npx skills add LearnPrompt/vibecoding-humanizer -l`：从 `https://github.com/LearnPrompt/vibecoding-humanizer.git` 克隆，识别到 1 个 Skill：vibecoding-humanizer。
- `npx skills add LearnPrompt/vibecoding-humanizer --skill vibecoding-humanizer -a claude-code -y`：安装到 `./.claude/skills/vibecoding-humanizer`，34 个文件，与仓库 `diff -rq -x .git` 一致。
- 旧地址 `github.com/LearnPrompt/carl-ui-humanizer` 返回 301 跳转到新地址，旧 clone 地址仍可用。
- 不带参数的交互式 `npx skills add LearnPrompt/vibecoding-humanizer` 只验证了能找到 Skill，交互选择 Agent 那一步未自动化测试。

### 规则选择（真实 Agent 观察，非静态推演）

在上面的临时项目里用 Claude Code（`claude -p --model sonnet`，只读工具）加载已安装的 SKILL.md，给 6 个请求只做路由判断：

| 请求 | Agent 选择 | 预期 |
|---|---|---|
| Three.js 浮空岛树在飘，要保留 low-poly | 3d；读 mode-3d.md；提醒 low-poly 是用户风格 | ✓ |
| 多色扁平插画 SVG 导出 | svg；提醒不要默认改 currentColor、不删有意义背景 | ✓ |
| Canvas showreel 转场像 PPT | html；读 mode-html + code-animation；不套 ui 减动效 | ✓ |
| 后台首页太 AI，品牌规定 Inter | ui；品牌字体优先于默认禁忌 | ✓ |
| HTML 动态海报 + SVG 边框动画（混合） | html 主 + svg 副；标题文本层不能当装饰清理 | ✓（曾多读 code-animation.md，已在路由表写明只限代码动画） |
| HTML 落地页嵌 3D 模型（混合） | ui 主 + 3d 副；场景光影按 3d，不套 ui 少阴影 | ✓ |

这只验证了**读取哪套规则**，没有让 Agent 实际改场景、SVG 或页面并对比效果；四个案例的前后效果来自作者此前在商汤小浣熊里的实测，不是本轮重跑。

### 仍未验证

各宿主（Codex、Cursor 等）自动发现；用 0.3.0 规则实际改稿后的视觉效果；浏览器交互与窄屏。
