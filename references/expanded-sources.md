# 新增来源：原句、中文与实施边界

本文件补充0.1.1漏掉的实质材料。完整来源状态见[来源覆盖](source-coverage.md)；编辑后的执行提示语见[提示语库](prompt-library.md)。没有英文原文的中文帖，不反译成所谓英文原文。

## 海總理：网页审美自审

[原帖](https://www.threads.com/@the.oceanic.official/post/Dd5QpPcmqow)，本轮读取2026-11-05公开页面的核心中文提示。

原生中文短摘录：“品質標準以 awwwards、webby awards、FWA 獲得獎項的程度為目標”。

其余意思转述：通过自查反复改善，直到达到所设品质目标。它与S4英文八维提示主题相近，但属于另一条收藏，不是同一原文的中译。

本Skill采用明确参考、逐维检查和修改后核对；不把获奖标准套到所有后台，也不继承无界循环。可执行版本是P12，属于编辑适配。

## 纸票：完整原提示已核读，公开包保留摘要与原文入口

[原帖](https://www.threads.com/@prompting_lab/post/Dex8TMUE9LD) · [完整英文PROMPT.md](https://github.com/Sam1983Aing/ticket-tear/blob/main/PROMPT.md) · [演示](https://sam1983aing.github.io/ticket-tear/)

英文短摘录：

> Build an interactive 3D physical paper "Ticket Tear" event checkout component

中文对应：制作一个可交互的3D实体纸张风格“撕票”活动结账组件。

本轮完整读过原提示，其五部分中文摘要如下；这是摘要，不是逐句全译：

1. 舞台与版式：暖灰白画廊背景、细点阵与柔光，结账选择器和立体票面组成布局，并设暗色主题。
2. 卡纸物理：强调抗弯刚度，以网格和约束建立弯折，独立定义能断裂的票根接缝，避免像软布。
3. 交互反馈：拖拽、倾斜、翻面、沿孔线撕裂；断开的票根下落，主体回弹，更新状态并支持重置。
4. 材质：纸张正反纹理、镭射箔、压印与打孔；反光随视角和弯曲后的表面法线改变。
5. 声音：纤维断裂与完成状态有对应程序音效，提供物理调试观察方式。

原库未确认再分发许可证，因此本包不全文转载这份长提示或完整翻译。原文仍可通过上方链接阅读。可迁移的是“用可观察的材料、动作与反馈规定质感”，不是强制所有UI使用3D物理。

## 互动粒子人像：英文入口说明

[原帖](https://www.threads.com/@dmitriyinin/post/DexX-SSCdw1)的作者引用回复指向 [particle-self](https://motionsites.ai/?prompt=particle-self)。

英文原句：“Want to build sites like this? Here's the prompt”

中文对应：“想做这样的网站？提示词在这里。”

这是入口说明，不是完整生成提示。完整particle-self提示尚未读取，不能从黑底、点云人像等演示画面补造原文。已看旧离散帧可作为独特主视觉和滚动叙事的参考，不证明全站可用性。

## 五个设计参考站的英文用途

[原帖](https://www.threads.com/@textura.eu/post/De2UaSjkVVC)为英文清单；短语对照如下，不是五段操作提示词。

| 站名 | 原文用途短语 | 中文 |
|---|---|---|
| getlayers.ai | prompts for cinematic 3D websites | 电影感3D网站提示词 |
| godly.website | award-winning websites | 获奖网站 |
| landdding.com | top notch landings | 优秀落地页 |
| fontinlogo.com | fonts behind brands | 品牌背后的字体 |
| 60fps.design | mobile UI animations | 移动UI动画 |

## Motion Library、MotionSites与Prompt Motion

- [Motion Library原帖](https://www.threads.com/@cz88422/post/De8WaTED83A)：按元件和时机寻找动作，预览再复制描述。它提供的是提示库入口，不等于本Skill已获得库中全部提示。
- [MotionSites视频来源](https://www.douyin.com/video/7701650803244797227)指向[官方Skill](https://github.com/Motionsites-AI/claude-skill)。本轮重看保存视频采帧，画面中的中文制作要求右侧被原片裁切，不能补全成原句。可确认的方法方向是参考、素材、构建规格和截图复查；本包没有安装、试跑或复制整套第三方Skill。
- [Prompt Motion原帖](https://www.threads.com/@reyne7_/post/DeRL329jDwP)：动效案例附提示词或Skill的资源入口。本Skill不把作者提到的历史数量当当前数量，也没有收录全站提示语。

## 风格词与动效术语

七种风格、两种艺术方向和六组滚动关系的原词及中文见[风格与动效词表](aesthetic-reference.md)。它们放在审美入口中实际使用，而不是仅作为末尾参考链接。

## 统一图标语言：中文原帖与对照图

[刘勿锋即刻原帖](https://m.okjike.com/originalPosts/68444463dfa0f1ef3adbbf9b)的中文提示短摘录：“不要用mac自带的emoji”。作者完整意思是让模型改用iconfont等平台的Web图标。本轮读到原帖并逐张查看前后两图：从混杂彩色emoji改成统一线性图标，仍保留柔和彩色底块和圆角。

这里不是要求删除所有图标、颜色或卡片。实施适配：先沿用项目已有图标系统，统一笔画、尺寸、光学对齐与语义；没有图标库时可在现有能力内用文字或本地图形，不为执行此建议擅自联网加载或新增依赖。这是原生中文提示，没有英文原文可补。

## 设计图还原与审美改编要区分

[归藏的即刻案例](https://m.okjike.com/originalPosts/691cade4d9abb9785d3c07f3)本轮正文与唯一主图已核读。它展示设计稿与生成稿，原图可见内容和区块比例变化；英文界面示例文案不是提示词。作者关于模型效果的说法没有在本轮复现。

编辑适配：先明确是在忠实还原，还是允许重新设计。还原任务应按同视口对照网格、间距、字体、颜色、素材、真实内容与状态，新增区块单独说明。不能因为“更好看”就补造业务数据或改变功能。

## 较早的资源方法

- [Jackywine原帖](https://x.com/jackywine/status/2046815560735076469)的滴答转存明确列出 [dark.design](https://www.dark.design/) 与 [footer.design](https://www.footer.design/)；本轮两站可读。适合分别找暗色风格与页脚组件参考，不是两段已恢复提示词。
- [GeoBuild收藏来源](https://v.douyin.com/otwZisj-gmc/)有完整转存文字，方法是选组件、查看效果、复制对应Prompt、用于自己的项目。但规范官网、具体Prompt及原视频图片仍未恢复。没有把标题中的历史模板数量或免费说法当当前事实。
