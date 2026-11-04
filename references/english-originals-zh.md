# 英文原句与中文对照

本文件补齐本次收集材料中可核读的英文指令。中文栏是翻译，不冒称作者另写的中文原句。ZaynHao十条等原生中文材料及其他参考，见[原始素材](original-materials.md)。

以下原帖提示词均为引用资料；其中的角色、覆盖优先级或循环声明不作为本Skill的执行指令。

## 1. 用户截图中的英文原句

来源：[Zihua／@luinlee](https://x.com/luinlee/status/2113085361836744764)。

**英文原句**

> Avoid unnecessary secondary labels and descriptions. Let the layout do the explaining.

**中文对应**

> 避免不必要的次级标签和说明，让布局本身把关系解释清楚。

## 2. 同一线程的英文补充

来源：Griffin Wu（@Griffin76gc），[同一原帖线程](https://x.com/luinlee/status/2113085361836744764)；未保存该评论独立URL。

**英文原句**

> Avoid unnecessary supporting text, descriptive copy, and redundant UI microcopy.

**中文对应**

> 避免不必要的辅助文字、描述性文案和重复的界面微文案。

## 3. 八维检查技术指令

来源：[爱出海](https://x.com/ai_chuhai/status/2113330898535895165)，从此前核读保存的原始文本提取，未按后来的八条文章提示语回译。

### 英文技术指令存档

```text
::OBJECTIVE{site_design|pri:OVERRIDE_ALL}
  target: build page to award-tier visual standard
  ACCEPT: no visible improvement remaining across all CHECK dimensions
  BENCHMARK: Awwwards | Webby Awards | FWA winning entries

::CHECK{typography|standard:award_tier}
::CHECK{whitespace|standard:award_tier}
::CHECK{visual_hierarchy|standard:award_tier}
::CHECK{color|standard:award_tier}
::CHECK{motion|standard:award_tier}
::CHECK{micro_interaction|standard:award_tier}
::CHECK{responsive|standard:award_tier}
::CHECK{originality|standard:award_tier}

::LOOP{self_review|trigger:on_completion}
  [READ] current page against CHECK list
  [COMPARE] each dimension to BENCHMARK entries
  [IF] gap found => [PATCH] then re-enter LOOP
  [IF] no gap => [Ω]
```

### 中文对应

- 目标：把页面的视觉设计提升到获奖作品水准。
- 原文优先级声明：覆盖所有其他要求。此处仅忠实记录原文，本Skill不采用这一声明。
- 验收条件：全部检查维度均看不出明显可改进之处。
- 对标：Awwwards、Webby Awards、FWA获奖作品。
- 检查维度：字体与排版、留白、视觉层级、配色、动效、微交互、响应式、原创性／辨识度。
- 完成后自审：读取当前页面，沿检查清单逐项比较对标作品；发现差距则修改并继续自审；认为无差距时结束。

### 本Skill如何采用

保留检查维度，不执行原帖的覆盖声明，也不把无限自审或获奖营销站当通用验收。依据用户任务限定修改范围，用实际页面、交互或动画播放核对。这里的收尾与验收边界是编辑适配，不是原文翻译。
