# 来源覆盖与未完成部分

核对日期：2026-11-05。0.2.0修复0.1.1仅覆盖一周素材、偏重界面减噪的问题。

## 滴答检索范围

本轮逐个只读取得36个清单、收件箱，并将已完成接口按完成时间向前翻页至最后不足200条的一页。合并得到5530个唯一任务；按标题、正文、清单项检索196个候选，并补查UI/动效目录子任务。不按“近一周”截断，不把归档选题排除为无价值素材。接口返回范围不含已删除/不可访问任务，也不代表外链媒体全部可读。

关键词候选含写作去味、纯工具新闻、私人工作项等，不会全量发布或全部纳入UI规则。原始滴答导出、任务ID、登录态页面及媒体CDN参数均留本地。可读旧原始证据本轮重新核读，保留日期；没有把旧数据称作当天线上全量读取。

## 已核来源与剩余范围

| 编号 | 收藏/来源 | 读取状态 | 纳入内容或缺口 |
|---|---|---|---|
| S1 | [让布局解释／Zihua](https://x.com/luinlee/status/2113085361836744764) | 原文与截图重读 | 10/26原始正文与截图；本轮X403；两句英文及中文在english-originals-zh |
| S2 | [ZaynHao十条](https://x.com/zaynhao/status/2113456751915982917) | 原文＋两图重读 | 10/26完整转存、两张对照图与边框回复；主规则及P1–P6 |
| S4 | [英文八维DSL](https://x.com/ai_chuhai/status/2113330898535895165) | 原文＋引用图重读 | 原英文及中文保留；正向八维流程，P7–P12 |
| S5 | [五个参考站](https://www.threads.com/@textura.eu/post/De2UaSjkVVC) | 当前正文/回复＋旧采帧 | 五站英文用途对照；视频非逐帧核验 |
| S6 | [是朝朝两图审美拆解](https://www.douyin.com/note/7698653961314607739) | 两张原图逐图重读 | 艺术方向与ASCII/Lo-fi/Glitch；aesthetic-reference |
| S7 | [Lemomo风格改编](https://x.com/lemomo_ai/status/2113195080517562646) | 旧正文＋八图重读 | 小互转引原文；核心/可变项/代价方法，向UI迁移须标编辑适配 |
| T1 | [中文网页自审](https://www.threads.com/@the.oceanic.official/post/Dd5QpPcmqow) | 当前正文与可见回复 | 中文原生；当前主帖无附图/视频；expanded-sources |
| T2 | [Motion Library](https://www.threads.com/@cz88422/post/De8WaTED83A) | 旧作者串文＋当前官网说明 | 当前主帖明确受众限制；使用11/01原始串文，媒体未核；不宣称读取全库 |
| T3 | [粒子人像](https://www.threads.com/@dmitriyinin/post/DexX-SSCdw1) | 当前正文/回复＋旧采帧 | particle-self完整提示未取得；入口说明不冒充生成提示 |
| T4 | [纸票交互](https://github.com/Sam1983Aing/ticket-tear/blob/main/PROMPT.md) | 完整英文提示在线核读＋旧采帧 | 公开包为短摘录、中文摘要与原文链接；非全译 |
| T6 | [Designeer](https://www.designeer.xyz/) | 官网403 | 资源入口，未读官网图片和具体提示 |
| T7 | [ASCII鲨鱼](https://www.threads.com/@ethansavemoneydairy/post/Dev32TMgD5x) | 当前正文/回复＋旧采帧 | 演示案例；源码stackedlol/ascii-sharks；无通用去味提示 |
| T8 | [六组滚动术语](https://www.threads.com/@ai_cpocoder/post/DePUuXsDxYq) | 当前正文＋视频11帧 | 六组完整中英文术语收录，保留原影片署名 |
| T9 | [Prompt Motion](https://www.threads.com/@reyne7_/post/DeRL329jDwP) | 当前正文＋主图 | 案例图库截图无额外长提示语；未读取全站提示库 |
| V1 | [大师级UI](https://www.douyin.com/video/7700643897349047675) | 旧原片采帧与正文重读 | THE NOCTURNO EXPERIENCE；未找到可靠独立站址，无完整构建提示 |
| V2 | [MotionSites Skill演示](https://www.douyin.com/video/7701650803244797227) | 旧原片采帧＋官方README | 视频中文要求右侧裁切；不补造成完整原句 |
| V4 | [随手拍动态海报](https://www.douyin.com/video/7693081869592903114) | 旧原片采帧重读 | 内容决定分割/遮罩/运动；案例不是原文提示词 |
| V5 | [七种设计风格](https://www.douyin.com/video/7693225096949379007) | 旧原片14帧重读 | 七个画面英文词组及中文收录 |
| V6 | [辣味章鱼参考网站](https://www.douyin.com/video/7684966275768290767) | 当前正文＋原视频采帧 | 网站名从画面核对，收录到aesthetic-reference |
| V7 | [Neuroblue灵感](https://www.douyin.com/video/7670523649916489006) | 当前正文＋原视频采帧 | 网站名从画面核对，收录到aesthetic-reference |
| V8 | [WorkBuddy](https://www.douyin.com/video/7698693814705245455) | 当前正文＋原视频采帧 | 确认是100项写作去味目录；排除UI规则 |
| V9 | [4个审美网站](https://www.xiaohongshu.com/discovery/item/6abaa8f5000000000a025343) | 当前不可读 | 原帖跳转错误300031并提示App访问；不猜四站名称 |
| V10 | [动效描述02](https://www.douyin.com/video/7684175267400650022) | 当前正文＋原视频采帧 | 五组完整双语动作名称已收录 |
| X8 | [动效名称与案例](https://x.com/vista8/status/2077372385788150184) | 滴答完整转存正文＋当前NameThatUI | 两张原配图未找到；名称词典方向已纳入 |
| X9 | [Variant审美探索](https://x.com/dashiaixz/status/2115758941540176144) | 11/01原始正文重读 | 推荐社区而非独立提示语 |
| X10 | [Vibe Coding特性](https://x.com/adrianpunk115/status/2099772129478869309) | 当前403 | 未读正文，不编造提示 |

## 历史收藏补充

141条较早已完成候选逐项检查了保存的标题、正文和检查项，排除写作、新闻、运营、内部待办等误命中，保留邻接视觉资料和无法恢复的来源。原始逐项账本只留本地，不公开私人任务内容。当前明确补入：

| 来源 | 原文/图片范围 | 落实位置 |
|---|---|---|
| [Anthropic前端审美](https://baoyu.io/translations/improving-frontend-design-through-skills) | 官方文章及MIT cookbook完整核读；三段英文逐字比对固定版本 | anthropic-prompts-en-zh.md；主Skill审美入口 |
| [统一图标](https://m.okjike.com/originalPosts/68444463dfa0f1ef3adbbf9b) | 原帖正文、前后两张原图均核读；页面工具缓存不代表当日帖态 | expanded-sources.md、P4 |
| [设计图还原案例](https://m.okjike.com/originalPosts/691cade4d9abb9785d3c07f3) | 当前正文、唯一主图；无完整提示词 | expanded-sources.md、P14 |
| [暗色与页脚参考](https://x.com/jackywine/status/2046815560735076469) | 完整转存与当前dark.design/footer.design；非提示词 | expanded-sources.md |
| [GeoBuild](https://v.douyin.com/otwZisj-gmc/) | 完整转存；具体Prompt、官网规范地址及原视频图片缺失 | 只保留资源方法，不猜站内提示 |

### 历史未读内容仍单列保留

以下条目不是新规则来源；没有用相似内容替代它们。无URL图片便笺仅能记录缺口，不能制造原帖。

| 收藏 | 原文入口 | 当前缺口 |
|---|---|---|
| ego 复刻网页｜视觉采样｜ | [原链接](https://x.com/t20000622yy/status/2092586675604226423) | ego 网页复刻/视觉采样相关；正文空，仅 X 链接，本次原帖403。关联子任务只是产品制作链接，不提供提示语。 |
| goodcase ui | [原链接](https://www.threads.com/share/BAOQV01z60/) | 已定位adsafayet原帖，元数据只有模型署名及Prompt指引；无登录页面未显示提示回复。 |
| 我把自己的审美，做成高级感设计skill🎨 | [原链接](https://www.xiaohongshu.com/discovery/item/6a94e900000000000a008bcf) | 当前无登录浏览器访问返回300031并引导App扫码；正文、图片未取得，不猜提示语。 |
| GitHub 上值得收藏的 4 个前端动效库 | [原链接](https://v.douyin.com/NykkrJ9h3XU/) | 正文与自动章节已读，章节列Lenis/GSAP/Vanta/React Bits；媒体403且播放器登录遮挡，原画面未取得。 |
| Vibe Coding 必备 UI 网站：从夯到拉 | [原链接](https://www.xiaohongshu.com/explore/69eb48f90000000036019bf6) | 当前无登录浏览器访问返回300031并引导App扫码；正文、图片未取得，不猜提示语。 |
| vibe coding idea | 没有可恢复原帖URL | 仅 vibe coding idea 标题和滴答图片路径；图片未取得，无法判断是否审美提示语。 |
| AI/Vibe Coding博客精选 [11月版 | [原链接](https://www.xiaohongshu.com/discovery/item/69391aa4000000001e02de82) | 当前无登录浏览器访问返回300031并引导App扫码；正文、图片未取得，不猜提示语。 |
| nano的网页互动特效 | [原链接](https://x.com/EHuanglu/status/1995887857920344404) | nano 网页互动特效仅 X 链接，无提示语，保留待核。 本次公开X读取403。 |
| vibe coding增强 | 没有可恢复原帖URL | 正文称七条补充性 Vibe Coding 提示语，实质内容在两张滴答附件，尚未取得图片；不能当已读，也不能直接排除。 |
| Kimi K2思考模型来了!实测3分钟做精美网页，IMO数学题翻车 | [原链接](https://mp.weixin.qq.com/s?__biz=MzA4MTQ4NjQzMw%3D%3D&mid=2652792092&idx=1&sn=f83eaff9d7912d6b0cc6b7b5b87566d4) | 恢复真实文章定位参数后单次请求仍为环境验证页；正文和图片未读，未绕过验证。 |
| 一招解决AI总生成蓝紫色渐变网页 | [原链接](https://www.xiaohongshu.com/discovery/item/690872d90000000005001a94) | 当前无登录浏览器访问返回300031并引导App扫码；正文、图片未取得，不猜提示语。 |
| DeepSeek V3.1 前端审美增强，我用它做了个产品 | [原链接](https://mp.weixin.qq.com/s?__biz=MjM5ODU1MzQzOQ%3D%3D&mid=2451427280&idx=1&sn=3ec80f2b36a3560d88c39e86113a66f9) | 恢复真实文章定位参数后单次请求仍为环境验证页；正文和图片未读，未绕过验证。 |
| 实测!用AI一句话生成网页，轻松打造专属网站 | [原链接](https://mp.weixin.qq.com/s?__biz=MzkxNzYzODgwNw%3D%3D&mid=2247490693&idx=1&sn=a54ddb30542485d7e3036b784a5f9855) | 恢复真实文章定位参数后单次请求仍为环境验证页；正文和图片未读，未绕过验证。 |
| 网页/PPT/3D演示...Claude3.7和Gemini2.5 Pro 硬碰硬 (附7大场景提示语 & 缺陷整理 | [原链接](https://mp.weixin.qq.com/s?__biz=Mzg3MTk3NzYzNw%3D%3D&mid=2247495546&idx=1&sn=493b85f77fbdb05810fdc0c8df42d006) | 恢复真实文章定位参数后单次请求仍为环境验证页；正文和图片未读，未绕过验证。 |
| 网页copy 软件 | [原链接](https://x.com/vista8/status/1931130439558898118) | 网页copy软件的X链接，可能是视觉采样工具；未读正文，不当成提示语。 本次公开X读取仅返回零行空壳。 |
| ，Claude3.7和Gemini2.5Pro硬碰硬（用八项真实能力横评 | 没有可恢复原帖URL | Claude/Gemini八项比较提纲含网页、原型、PPT；与150可能同内容，正文只有框架，七场景提示语未在任务内。 |
| gemini 做网页 特斯拉财报 | [原链接](https://x.com/op7418/status/1914872664256340402) | 财报网页可视化的X与即刻链接，未保存正文；保留数据展示案例线索，无已证实的可复用提示语。 本次X读取403；即刻由另一子任务核读。 |
| 一键搞定、100%成功、80老太都能操作，宝藏提示词将你的任何内容生成网页 | [原链接](https://mp.weixin.qq.com/s?__biz=MzU0MDk3NTUxMA%3D%3D&mid=2247487623&idx=1&sn=dcb4ec6d7aee925242c57d4d4183ea93) | 恢复真实文章定位参数后单次请求仍为环境验证页；正文和图片未读，未绕过验证。 |
| UI design | 没有可恢复原帖URL | 2024 UI design 任务正文仅换行，没有URL、附件、检查项或提示语；现有记录无法恢复来源。 |

另外，当前“Vibecoding案例”仅有[苍何X链接](https://x.com/canghe/status/1995710857247080719)，本轮403；“去AI味”目录新增Grok分享不可读，不能拿11/01另一份Grok对话替代。旧Grok两轮资料仅用作资源线索，不作为原创提示词或效果证明。

“vibe coding增强”的两张图片及“vibe coding idea”的一张图片在滴答只返回相对附件路径，本地未找到对应文件。2024“UI design”记录为空。这些缺失与环境验证、受众限制分开记录，不称已完成原图核读。

## “已读”不等于“实测”

原帖说明、截图文字、视频离散采帧、完整提示语文件与实际操作分别记录。案例的模型名称、效果或首次成功是作者声称；本Skill未据此声明某模型已复现，也不报告去味百分比。动态网站的下游数百条提示词不属于本次整库复制范围。

不能访问或缺少图片清单的来源不会消失：保留入口与缺口，未取得的文字不猜补。这里明确列出未读部分，因此本版不称“全部原帖和图片均已读全”。
