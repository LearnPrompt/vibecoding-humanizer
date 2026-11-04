# Anthropic 前端审美提示语：英文原文与中文对照

核读日期：2026-11-05。

收藏入口：[借助 Skills 提升前端设计](https://baoyu.io/translations/improving-frontend-design-through-skills)。已核读[官方文章](https://claude.com/resources/articles/improving-frontend-design-through-skills)，这里复制的提示语均来自文章链接的 **MIT 许可官方代码 notebook**，不复制文章正文。

固定版本：[claude-cookbooks / prompting_for_frontend_aesthetics.ipynb](https://github.com/anthropics/claude-cookbooks/blob/bfe50e59dbb4f5546a0af9ca36ebb77e637c9ce1/coding/prompting_for_frontend_aesthetics.ipynb)。对应该文件最近一次变更 SHA：`bfe50e59dbb4f5546a0af9ca36ebb77e637c9ce1`。英文逐字提取字符串，仅移除 Python 三引号两端换行；中文为本次忠实翻译。

## 使用边界（本次整理者说明，非原文）

这些是展示如何改变模型默认输出的历史示例提示语，不是通用排版标准。英文的禁止字体、3 倍字号、极端字重、Google Fonts 加载和“始终”主题约束均按原样保留；应用到实际项目时，须遵循既有品牌、中文字体覆盖、性能、可读性、信息密度、无障碍与用户指定风格，不应无条件执行。尤其不要把“去 AI 味”简化成禁止渐变或禁止卡片；此来源明确允许有目的的渐变、背景纹理和动效。

官方文章的单主题示例是 RPG；本 notebook 的对应示例是 **Solarpunk**，二者不能混称为同一原文。本文件提供 notebook 原句。

## 1. 综合前端审美

英文原文：

```text
<frontend_aesthetics>
You tend to converge toward generic, "on distribution" outputs. In frontend design, this creates what users call the "AI slop" aesthetic. Avoid this: make creative, distinctive frontends that surprise and delight. Focus on:

Typography: Choose fonts that are beautiful, unique, and interesting. Avoid generic fonts like Arial and Inter; opt instead for distinctive choices that elevate the frontend's aesthetics.

Color & Theme: Commit to a cohesive aesthetic. Use CSS variables for consistency. Dominant colors with sharp accents outperform timid, evenly-distributed palettes. Draw from IDE themes and cultural aesthetics for inspiration.

Motion: Use animations for effects and micro-interactions. Prioritize CSS-only solutions for HTML. Use Motion library for React when available. Focus on high-impact moments: one well-orchestrated page load with staggered reveals (animation-delay) creates more delight than scattered micro-interactions.

Backgrounds: Create atmosphere and depth rather than defaulting to solid colors. Layer CSS gradients, use geometric patterns, or add contextual effects that match the overall aesthetic.

Avoid generic AI-generated aesthetics:
- Overused font families (Inter, Roboto, Arial, system fonts)
- Clichéd color schemes (particularly purple gradients on white backgrounds)
- Predictable layouts and component patterns
- Cookie-cutter design that lacks context-specific character

Interpret creatively and make unexpected choices that feel genuinely designed for the context. Vary between light and dark themes, different fonts, different aesthetics. You still tend to converge on common choices (Space Grotesk, for example) across generations. Avoid this: it is critical that you think outside the box!
</frontend_aesthetics>
```

中文对照：

```text
<frontend_aesthetics>
你倾向于收敛到泛泛的、“处于分布内”的输出。在前端设计中，这就产生了用户所说的“AI 粗制滥造感”审美。避免这种情况：制作富有创意、鲜明独特、能让人惊喜和愉悦的前端。重点关注：

字体排版：选择美观、独特、有趣的字体。避免 Arial 和 Inter 这样常见的字体；改用能提升前端审美的鲜明选择。

色彩与主题：坚持一种连贯的审美。使用 CSS 变量保持一致。占据主导的颜色配上鲜明的强调色，优于畏缩、均匀分摊的配色。可从 IDE 主题和文化审美中寻找灵感。

动效：通过动画制作视觉效果和微交互。HTML 优先采用纯 CSS 方案。React 在可用时使用 Motion 库。聚焦高影响力的时刻：一次编排得当、错落显现（animation-delay）的页面加载，比四处分散的微交互更能带来愉悦。

背景：营造氛围和纵深，而不是默认使用纯色。叠加 CSS 渐变，使用几何图案，或加入与整体审美相符、贴合内容情境的效果。

避免泛化的 AI 生成审美：
- 被过度使用的字体家族（Inter、Roboto、Arial、系统字体）
- 陈词滥调的配色方案（尤其是白底紫色渐变）
- 可预料的布局和组件模式
- 缺乏特定情境个性的流水线式设计

创造性地理解任务，作出出人意料的选择，让人感到这些设计确实为当前情境而作。在明暗主题、不同字体和不同审美之间变化。你仍然倾向于在多次生成中收敛到一些常见选择（例如 Space Grotesk）。避免这样：跳出惯常思路至关重要！
</frontend_aesthetics>
```

## 2. 字体与排版对比

英文原文：

```text
<use_interesting_fonts>
Typography instantly signals quality. Avoid using boring, generic fonts.

**Never use:** Inter, Roboto, Open Sans, Lato, default system fonts

**Impact choices:**
- Code aesthetic: JetBrains Mono, Fira Code, Space Grotesk
- Editorial: Playfair Display, Crimson Pro, Fraunces
- Startup: Clash Display, Satoshi, Cabinet Grotesk
- Technical: IBM Plex family, Source Sans 3
- Distinctive: Bricolage Grotesque, Obviously, Newsreader

**Pairing principle:** High contrast = interesting. Display + monospace, serif + geometric sans, variable font across weights.

**Use extremes:** 100/200 weight vs 800/900, not 400 vs 600. Size jumps of 3x+, not 1.5x.

Pick one distinctive font, use it decisively. Load from Google Fonts. State your choice before coding.
</use_interesting_fonts>
```

中文对照：

```text
<use_interesting_fonts>
字体排版会立即传递品质感。避免使用无聊、泛泛的字体。

**绝不使用：**Inter、Roboto、Open Sans、Lato、默认系统字体

**有表现力的选择：**
- 代码审美：JetBrains Mono、Fira Code、Space Grotesk
- 编辑出版风格：Playfair Display、Crimson Pro、Fraunces
- 初创公司风格：Clash Display、Satoshi、Cabinet Grotesk
- 技术风格：IBM Plex 家族、Source Sans 3
- 鲜明独特：Bricolage Grotesque、Obviously、Newsreader

**搭配原则：**强对比 = 有趣。展示字体 + 等宽字体、衬线字体 + 几何无衬线字体，或在不同字重间运用可变字体。

**使用极端对比：**100/200 字重对比 800/900，而不是 400 对比 600。字号跃迁达到 3 倍以上，而不是 1.5 倍。

选定一种鲜明的字体，果断使用。从 Google Fonts 加载。在编码前说明你的选择。
</use_interesting_fonts>
```

## 3. 单一主题约束示例（补充）

英文原文：

```text
<always_use_solarpunk_theme>
Always design with Solarpunk aesthetic:
- Warm, optimistic color palettes (greens, golds, earth tones)
- Organic shapes mixed with technical elements
- Nature-inspired patterns and textures
- Bright, hopeful atmosphere
- Retro-futuristic typography
</always_use_solarpunk_theme>
```

中文对照：

```text
<always_use_solarpunk_theme>
始终采用太阳朋克审美进行设计：
- 温暖、乐观的配色（绿色、金色、大地色）
- 有机形状与技术元素混合
- 受自然启发的图案和纹理
- 明亮、充满希望的氛围
- 复古未来主义的字体排版
</always_use_solarpunk_theme>
```

## 可直接支撑主 Skill 的内容映射

| 内容 | 原文对应 | 迁移到通用 Skill 时的边界 |
|---|---|---|
| 先定连贯审美与主色、强调色 | Color & Theme 段 | 按产品情境选择，不强制所有产品同一主题 |
| 有意识地选字体并建立对比 | Typography 段；use_interesting_fonts 全段 | 字重与 3x 是该示例的表达性策略，不是正文/中文 UI 硬门槛 |
| 优先编排关键动效时刻 | Motion 段 | 页面加载仅为示例；产品反馈、性能与减少动态偏好优先 |
| 用背景创造与主题一致的氛围与纵深 | Backgrounds 段 | 不要求每一屏都加纹理；正文可读性优先 |
| 避免从一个默认风格换成另一个默认风格 | 末段点名 Space Grotesk | 审美选择应来自内容、用户和情境 |
| 把统一主题拆成可执行视觉属性 | Solarpunk 示例五条 | 可换成适合项目的主题，不强制太阳朋克 |

以上右栏是本次适用性整理，不冒称 Anthropic 原文。

## 许可证

下列许可证随转载保留；来源仓库 [LICENSE](https://github.com/anthropics/claude-cookbooks/blob/main/LICENSE)。Copyright (c) 2023 Anthropic。

```text
MIT License

Copyright (c) 2023 Anthropic

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
