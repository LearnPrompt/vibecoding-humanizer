# 风格词、动效词与参考选择

以下区分原文词汇与编辑解释。词汇能帮助描述目标，但不能代替内容、构图与实现规格。来源覆盖与缺口见[核读清单](source-coverage.md)。

## 七种视觉方向：英文原词与中文

来源：[饼饼干的原视频](https://www.douyin.com/video/7693225096949379007)。2026-11-01保存约7秒视频；本轮重新目视其14帧采样，七个英文词组均出现于画面。它们是风格词，不是七段完整提示语。

| 英文原词 | 中文对应 | 可描述的视觉要素（编辑解释） |
|---|---|---|
| ASCII and pixels | ASCII字符与像素 | 字符构形、点阵、像素图像 |
| sketch and scribble | 素描与涂鸦 | 手绘线条、速写、笔触 |
| digital impressionism | 数字印象派 | 色块、碎笔触、光色氛围 |
| morphing objects | 变形物体 | 流动形态、体块与形变 |
| lomo imagery | Lomo影像 | 胶片色偏、颗粒、日常摄影 |
| generative art | 生成艺术 | 算法线条、几何、重复规则 |
| shades of off-white | 米白／近白色的不同层次 | 细微色差、纸面与编辑式排版 |

使用示例（编辑适配）：选“素描与涂鸦”时，说明线条用在插画还是边注、笔触粗细如何与字体搭配、哪些按钮保持标准形态；不要把所有正文变成难读手写字。

## 两种艺术风格拆解

来源：[是朝朝两张原图](https://www.douyin.com/note/7698653961314607739)，2026-10-26保存原图，本轮逐图重读。

- **Ayush Soni**：以网格和简洁字体建立秩序，再使用算法纹理、模块化几何、动态变化和鲜明色彩。原图包含渐变、半透明与混合媒材，不能推导为一律禁用这些手法。
- **enigmatriz**：复古数字、字符构形、实验拼贴，结合旧纸、复印颗粒与斑驳油墨。图中英文 `ASCII` 对应字符艺术，`Lo-fi` 对应低保真，`Glitch` 对应故障美学。

迁移到UI时，应说明哪个区域承担艺术表达，哪个区域保障阅读与操作；这属于编辑建议，原图不是产品可用性测试。

## 六组滚动关系：英文原词与中文

来源：[原帖](https://www.threads.com/@ai_cpocoder/post/DePUuXsDxYq)，2026-11-05正文与主媒体核读；10.517秒视频采样11帧，六组名称完整可读，画面注明原影片 @gabriell_lab。

| 英文原词 | 中文对应 |
|---|---|
| Scroll-triggered | 滚动到条件位置后触发播放 |
| Scroll-linked | 动画进度与滚动距离关联 |
| Parallax | 前后层以不同速度移动产生视差 |
| Sticky | 到达阈值后固定在容器边缘 |
| Scroll Snap | 滚动后吸附到指定位置 |
| Horizontal Scroll | 横向滚动；本帖例子将纵向输入映射成横向位移 |

不要混淆触发一次与持续跟随。提示语应说明对象、起止点、滚动停止时的状态，以及窄屏如何处理。实现细节依现有框架决定。

## 内容、品牌、材质怎样建立辨识度

- [随手拍动态海报](https://www.douyin.com/video/7693081869592903114)：从照片里的裂缝、雨滴、天空和路灯提炼分割、遮罩和运动。启发是让内容参与版式，不仅“背景图上盖卡片”。本轮看过旧采样联系表，未宣称逐帧完整播放。
- [THE NOCTURNO EXPERIENCE 演示](https://www.douyin.com/video/7700643897349047675)：有限的红、黑、米白，人物和瓶子等品牌图形，刷痕转场贯穿段落。适合借鉴统一视觉语言；没有确认独立站址，也没有确认视频叠字所称制作工具。
- [纸票交互](https://github.com/Sam1983Aing/ticket-tear)：材质、卡纸刚度、弯折、全息反光、撕裂与声音保持一致。它说明精致感也来自具体的物理反馈。完整原提示链接和摘要见[新增来源](expanded-sources.md)。

## 按实际任务选择参考入口

这些是收藏中的资源指向，不是“每次必须打开”的依赖，也不意味着已收录站内全部提示词。数量、价格和权限以使用时实际页面为准。

| 需要解决的问题 | 收藏指向的资源 | 怎样转成设计要求 |
|---|---|---|
| 3D或电影感首屏 | [GetLayers](https://getlayers.ai/)、[MotionSites](https://motionsites.ai/) | 提取主视觉、镜头、文字位置与滚动关系 |
| 找完整风格方向 | [Variant社区](https://variant.com/community)、[Godly](https://godly.website/)、[Landdding](https://landdding.com/) | 选具体页面，指出网格、密度、标题比例与内容关系 |
| 字体气质 | [Font in Logo](https://fontinlogo.com/) | 描述字形与比例，再检查中文兼容、授权及实际字长 |
| 手机交互节奏 | [60fps](https://60fps.design/) | 记录触发、过渡、停顿、完成状态 |
| 不知道效果叫什么 | [NameThatUI](https://namethatui.com/) | 先找组件或动效名，再描述自己的内容和状态 |
| 为具体元件找动作 | [Motion Library](https://kittenjam-motion-library.vercel.app/) | 按元件与时机选例子，预览后写明用在哪里、如何触发 |
| 动态字体与讲解画面 | [Prompt Motion](https://prompt-motion.com/) | 把案例与提示词区分开，不凭缩略图假造生成步骤 |
| 设计资源目录 | [Designeer](https://www.designeer.xyz/) | 本轮官网403，只保留入口，不补写未读的目录内容 |

以上来源映射：GetLayers等五站来自textura.eu；Variant来自dashiaixz；NameThatUI来自vista8；Motion Library来自cz88422；Prompt Motion来自reyne7_及旧Grok资源对话；Designeer为独立收藏。参考资源扩展不是英文原文翻译。

## 五种交互动效：画面中英原词

来源：[UI交互动效描述02](https://www.douyin.com/video/7684175267400650022)，本轮读取原帖及约34秒原视频，每2秒采帧核对五张完整标签。下表中英文均来自画面，非反译。

| 英文原词 | 中文原词 |
|---|---|
| CURSOR-DRIVEN GAZE TRACKING | 鼠标驱动的视线跟随 |
| SCROLL-DRIVEN PINNED HERO RECOMPOSITION | 滚动驱动的固定主视觉重组 |
| SCROLL-DRIVEN SECTION REVEAL AND CARD STACKING | 滚动驱动的章节覆盖与卡片堆叠 |
| CURSOR-DRIVEN MINIATURE SCENE PARALLAX | 鼠标驱动的微缩景观视差 |
| SCROLL-DRIVEN CHARACTER ORBIT ROTATION | 滚动驱动的角色环绕旋转 |

这些是可复用的效果描述词组，不是完整代码提示词。原片没有证明所有效果采用同一技术栈：不要从画面自行断定是实时3D、视频或图片序列。实施时继续说明对象、范围、起止状态与移动端行为。

## 两条参考网站收藏的具体内容

[辣味章鱼原片](https://www.douyin.com/video/7684966275768290767)本轮正文、章节与采帧交叉核对，五站为 [Minimal Gallery](https://minimal.gallery/)、[Land-book](https://land-book.com/)、[Noiced](https://noiced.com/)、[Made With Gsap](https://madewithgsap.com/effects/)、[Pinterest](https://www.pinterest.com/)。第三站自动字幕有拼写误差，以原视频地址栏的noiced.com为准。它们分别用于找结构、页面类型、视觉风格、动作细节和主题图像；不要把五种风格直接拼成一页。

[Neuroblue原片](https://www.douyin.com/video/7670523649916489006)本轮正文、章节与采帧可确认五项：Awwwards、React Bits、MotionSites、GitHub Trending、Product Hunt。这里既有视觉参考与组件，也有产品创意入口；不是五条英文构建提示。按“视觉、组件、产品交互”区分用途，再结合当前任务选择。

## MotionSites八类效果：官方英文与中文对应

来源：[官方README](https://github.com/Motionsites-AI/claude-skill)，由[赛博小凡视频](https://www.douyin.com/video/7701650803244797227)指向。英文来自官方README延伸，中文为本包对应翻译，不冒充视频里的英文原句；视频的中文整段提示右侧裁切，仍不能补全。

| 官方英文术语 | 中文对应 |
|---|---|
| seamless video loops | 无缝视频循环 |
| liquid glass | 液态玻璃 |
| word-by-word blur headlines | 逐字模糊标题 |
| mouse-scrubbed video | 鼠标控制视频进度 |
| spotlight reveals | 聚光灯显现 |
| depth carousels | 纵深轮播 |
| scroll stories | 滚动叙事 |
| real 3D models | 真实3D模型 |

选择效果时说明它服务哪条内容或哪个操作，先做一个可观察的小样；这些是术语，不是本Skill已测试八种实现的声明。
