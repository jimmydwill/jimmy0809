## 1. 执行摘要（Executive Summary）

**产品**：黄嘉杰 · AI 驱动个人作品集网站
 **负责人**：黄嘉杰
 **状态**：草稿
 **最后更新**：2026-03-05

## 1.1 产品愿景

- 愿景一句话：
  - “一个让招聘方在 3 分钟内识别我价值、10 分钟内理解代表项目，并清晰看到我如何使用 AI 工具工作的互动式作品集网站。”sachinrekhi+1
- 目标用户与使用场景：
  - HR / 招聘专员：在筛选简历时，点击网站链接 3–5 分钟内做出继续推进或淘汰决策。community.showprowess+1
  - 用人经理 / 面试官：面试前浏览网站，选择 1–3 个项目作为面试重点；面试中打开网站作为“讲解提纲”。reddit+1
- 核心价值主张：
  - 用结构化、可视化案例代替“只写在简历上的一行项目”，帮助招聘方评估你的产品思维、执行深度和 AI 使用能力。theproductfolks+1
- 成功定义与指标（高层）：
  - 来自简历/LinkedIn 的访问中，≥ 70% 的访客访问时间 ≥ 3 分钟。
  - 每轮面试中，≥ 80% 的情况你会主动用该网站讲解项目，并得到“讲得很清晰”的正向反馈（主观统计）。[[redfishtech](https://www.redfishtech.com/recruiters-look-for-product-management-candidates/)]

## 1.2 战略对齐

- 支持的业务目标：
  - 提升简历转面试率、面试转下一轮/offer 率。
  - 在竞品候选人中形成明确差异化（特别是 AI 能力和复杂 B 端/金融项目经验）。sachinrekhi+1
- 解决的用户问题：
  - HR：缺少直观且省时的方式判断候选人是否“值得约面试”。[[community.showprowess](https://community.showprowess.com/t/when-hiring-do-you-look-at-pm-portfolios/3120)]
  - 用人经理：难以从简历中看到候选人的问题定义能力、完整产品过程和真实贡献。[[sachinrekhi](https://www.sachinrekhi.com/evaluating-a-product-managers-portfolio)]

## 1.3 资源需求与里程碑

- 资源：
  - 产品 / 文案 / 信息架构：你本人
  - 实现方式优先：零/低代码平台（Framer / Webflow / Notion + Super 等），需要前端支援时可临时找 1 位开发。wix+2
- 粗略时间线（可视化）：

```
text
gantt
    dateFormat  YYYY-MM-DD
    title  个人作品集网站实施计划

    section 规划
    PRD 和内容梳理        :a1, 2026-03-10, 5d
    IA 与线框图          :a2, after a1, 4d

    section 设计与搭建
    视觉风格与组件确定    :b1, after a2, 4d
    平台搭建与页面实现    :b2, after b1, 7d

    section 内容落地
    项目案例内容填充      :c1, after b2, 7d
    AI 能力展示模块完善    :c2, after c1, 3d

    section 发布与迭代
    内测与反馈收集        :d1, after c2, 4d
    正式发布              :d2, after d1, 1d
```

------

## 2. 问题陈述与机会（Problem & Opportunity）

## 2.1 问题定义

- 用户痛点：
  - HR 时间极少，通常只花几十秒扫简历，很难判断你在复杂项目中的真实角色。
  - 用人经理希望看到“问题–方案–执行–结果”的完整链路和你的具体决策过程，而非只看到“负责某项目”一句话。theproductfolks+2
- 量化影响（你可以根据实际情况填数字）：
  - 目前发送简历/LinkedIn 的点击进入率未知，面试官很少有额外材料参考。
  - 你在面试中需要花较多时间搭建项目背景，影响深挖问题的时间。

## 2.2 机会分析

- 市场与趋势：
  - 更多招聘方开始期待产品经理提交作品集/案例库，以弥补简历信息不足。theproductfolks+1
  - AI 辅助搭建网站、生成内容的工具成熟，可以低成本打造“AI 风格”个人站点。figma+1[[youtube](https://www.youtube.com/watch?v=hl1L7WI2ohc)]
- 差异化机会：
  - 大部分 PM 作品集仍偏静态，你可以通过“AI 使用剖析 + 可视化流程 + 数据结果”形成辨识度。

## 2.3 成功标准

- 业务向：
  - 投递的岗位中，附网站链接后，简历筛选通过率提升 X%。
  - 用人经理在面试中主动提到网站内容的比例 ≥ 50%。redfishtech+1
- 用户行为向：
  - 访问路径中，有 ≥ 60% 的访客打开至少 1 个项目详情页面。
  - AI 能力相关模块被点击/浏览的比例 ≥ 50%。

------

## 3. 用户需求与故事（User Needs & Stories）

## 3.1 用户画像

用人经理画像示例：

```
text
mindmap
  root((用人经理画像))
    背景
      职位: 产品总监/负责人
      时间: 每天可用于候选人的时间有限
    目标
      找到能独立负责复杂项目的 PM
      验证候选人 AI 与数据能力
    痛点
      简历高度同质化
      很难看出真实参与深度
      面试时间有限
    需求
      10 分钟内看懂2-3个项目案例
      清晰看到候选人“如何思考和决策”
      了解候选人如何使用 AI
```

你可以为 HR 再画一个类似的 mindmap。

## 3.2 用户旅程（当前 vs 未来）

**当前招聘方旅程（简化）：**

```
text
flowchart LR
  A[收到 PDF 简历] --> B[30-60 秒快速浏览]
  B --> C{是否匹配?}
  C -- 看不出项目深度 --> D[放弃/待定]
  C -- 勉强匹配 --> E[约初面]
  E --> F[面试中花大量时间讲背景]
  F --> G[剩余时间少, 难以深挖]
```

**未来有个人网站后的旅程：**

```
text
flowchart LR
  A[收到简历+网站链接] --> B[打开网站首页]
  B --> C[浏览 About & 能力矩阵]
  C --> D[打开1-2个项目案例页]
  D --> E{是否有兴趣?}
  E -- 项目清晰, 匹配度高 --> F[优先约面/提升评价]
  E -- 不合适 --> G[快速淘汰, 节省双方时间]
  F --> H[面试前再次浏览网站做准备]
```

## 3.3 核心用户故事

示例 1（HR）

- 作为一名 HR，我希望在 3 分钟内看到候选人的核心背景和 2–3 个代表项目入口，以便快速判断是否约面试。
- 验收标准：
  - 首页首屏包含：一句话简介、关键标签（行业/年限/AI）、3 个项目快捷入口。
  - 不超过 2 次滚动可以看到“关于我”和“代表项目列表”。

示例 2（用人经理）

- 作为一名用人经理，我希望在项目详情页看到清晰的“问题–方案–过程–结果–AI 使用方式”结构，以便我可以基于此深挖提问。
- 验收标准：
  - 每个项目详情页均包含这 5 个小节，标题统一。
  - 至少有 1–2 项客观指标（如效率、用户量、业务指标）展示结果。

------

## 4. 功能需求（Functional Requirements）

## 4.1 信息架构（站点结构）

用 mermaid 表达整体 IA：

```
text
flowchart TD
  Home[首页] --> About[关于我]
  Home --> Portfolio[项目作品集]
  Home --> AIShowcase[AI 能力专区]
  Home --> Blog[输出/文章]
  Home --> Contact[联系与简历下载]

  Portfolio --> Case1[案例1：投顾智能助理]
  Portfolio --> Case2[案例2：投顾一体化平台]
  Portfolio --> Case3[案例3：基金发行管理App]
  Portfolio --> CaseMore[更多项目]

  AIShowcase --> WorkflowAI[AI 在产品工作流中的使用]
  AIShowcase --> ToolStack[AI 工具栈]
  AIShowcase --> MiniDemo[AI side project/demo]
```

## 4.2 Must-have 功能（示例）

1）首页（Home）

- 内容：
  - 一句话简介（角色 + 年限 + 行业 + AI 能力）。
  - 能力标签（芯片：金融/B 端/电商/AI 等）。
  - 3 个代表项目卡片（卡片上展示项目名 + 一行结果 +“查看案例”按钮）。
- 交互：
  - 点击项目卡片跳转对应案例页。
  - 顶部导航固定，快速访问 About / Portfolio / Contact。

2）关于我（About）

- 内容：
  - 职业时间轴（招聘 → UI/UCD → 产品 → AI 产品）。
  - 能力矩阵（需求/架构/交互/UI/项目管理/AI 等）。
  - 证书：NPDP、PMP、高级 UI、AI 训练师等。
- 可视化示例：职业路径（mermaid）

```
text
timeline
  title 职业演进时间线
  2013 : 招聘专员 : 理解用人方与候选人匹配逻辑
  2015 : UI/视觉设计 : 打磨交互与界面设计能力
  2018 : UCD/产品设计 : B端/电商系统体验设计
  2019 : 产品经理 : 0-1 产品规划与跨部门协作
  2022 : 金融/投顾产品 : 复杂业务+风控场景
  2025 : AI+投顾与效率 : 智能助理、用户画像、AI 应用落地
```

3）项目作品集（Portfolio + Case 页面）

- 项目列表页：简要卡片列表，可按行业/能力筛选（可先简单做标签）。

- 项目详情页结构模板（每个项目复用）：

  1. 项目背景（业务场景、目标）
  2. 问题与挑战（问题拆解）
  3. 解决方案（架构/流程/关键设计）
  4. 执行过程与协同（你如何推动）
  5. 使用的 AI 能力（工具 + 用法 + 价值）
  6. 结果与复盘（数据 + 反思）

  示例：用 mermaid 画项目核心流程（以“投顾智能助理”为例）

```
text
flowchart LR
  UQ[投顾提出问题] --> NLP[AI 理解意图与实体]
  NLP --> DataFetch[调用内部数据/知识库]
  DataFetch --> Reasoning[模型生成回答与建议]
  Reasoning --> UIResp[前端以结构化方式展示结果]
  UIResp --> Feedback[投顾反馈/标注满意度]
  Feedback --> Improve[用于模型与规则迭代]
```

4）AI 能力专区（AI Showcase）

- 模块：

  - “我如何在日常产品工作中使用 AI”：
    - 调研（生成访谈提纲、竞品结构）
    - 文档（PRD 初稿、需求归类）
    - 设计（生成 IA 草案、交互方案建议）
    - 数据（日志分析、反馈聚类）[[productschool](https://productschool.com/blog/career-development/building-a-product-portfolio-with-ai)]

  可用 mermaid 画“产品工作流中 AI 的嵌入点”：

```
text
flowchart LR
  Req[需求输入] --> Research[业务/用户调研]
  Research --> Design[方案设计]
  Design --> Delivery[交付与验证]
  Delivery --> Iterate[复盘与迭代]

  subgraph AI_Usage[AI 使用节点]
    A1[AI: 访谈提纲/竞品结构]
    A2[AI: PRD 初稿/需求归类]
    A3[AI: 交互方案建议]
    A4[AI: 日志分析/反馈聚类]
  end

  Research -.-> A1
  Design -.-> A2
  Design -.-> A3
  Delivery -.-> A4
```

5）联系页（Contact）

- 内容：
  - 邮箱、微信二维码、LinkedIn。
  - “下载 PDF 简历”按钮。

## 4.3 Should/Could 功能

- Should：
  - 英文版页面（首页 + 关于我 + 2 个代表项目）。
- Could：
  - 为特定目标公司创建“定制项目页”，可通过单独 URL 分享。

------

## 5. 技术要求（Technical Requirements）

## 5.1 前后端与架构（简化）

- 若采用静态站点生成/可视化搭建工具，整体可以视为：

```
text
flowchart LR
  User[HR/面试官浏览器] --> CDN[静态资源/CDN]
  CDN --> Site[作品集前端站点]
  Site --> Analytics[埋点与分析服务]
```

- 若嵌入简单 AI Chat Widget（如第三方）：
  - 前端通过 JS 插件嵌入，后端由第三方服务提供。

## 5.2 性能与兼容

- 页面应在常见桌面/移动浏览器上正常显示。
- 首屏加载时间建议 ≤ 2 秒（在常见网络环境下）。

------

## 6. 用户体验要求（UX Requirements）

- 导航：
  - 顶部导航固定，任何页面 1 次点击能回到首页，2 次以内能到达任意项目详情。
- 信息层级：
  - 标题层级遵循 H1/H2/H3，确保结构清晰。

可以用 mermaid 描述一个典型浏览路径：

```
text
stateDiagram-v2
  [*] --> Home
  Home --> About: 点击“关于我”
  Home --> Portfolio: 点击“项目”
  Portfolio --> CaseDetail: 选择某个案例
  CaseDetail --> AIShowcase: 点击“AI 如何参与这个项目”
  CaseDetail --> Contact: 有兴趣后想联系候选人
  Contact --> [*]
```

------

## 7. 非功能需求（Non-functional）

- 可维护性：
  - 项目案例内容应易于更新（建议使用 CMS 或支持可视化编辑的平台）。wix+1
- 安全：
  - 仅展示可对外公开的内容，不泄露公司敏感数据。

------

## 8. 成功指标与分析（Metrics & Analytics）

- 埋点事件（示例）：
  - `view_home`, `view_about`, `view_case_x`, `click_ai_section`, `click_contact`, `download_cv`。
- 仪表盘：
  - 访问来源（简历、LinkedIn、微信等）。
  - 每个案例页的浏览次数和停留时间。

------

## 9. 实施计划（Implementation Plan）

前面的 Gantt mermaid 已给出。你可以在实际执行时，把日期细化到具体天，并按阶段检查：

- 阶段结束前：是否完成该阶段 Deliverables（PRD、线框、页面、内容、埋点测试）。

------

## 10. 风险与缓解（Risks & Mitigation）

用一个简单 mermaid 列出主要风险类型：

```
text
graph TD
  R[风险] --> RT[技术风险]
  R --> RB[业务/效果风险]
  R --> RC[内容合规风险]

  RT --> RT1[平台能力不足导致想要的交互难实现]
  RB --> RB1[招聘方实际使用率不高]
  RC --> RC1[项目内容涉及前公司敏感数据]
```

- 缓解示例：
  - RT1：优先选成熟平台（Framer/Webflow 等），必要时简化动效。
  - RB1：在简历/LinkedIn 里明显标出网站，并在面试自我介绍时主动引导。
  - RC1：用抽象化、数据脱敏方式描述结果（用范围/比例代替绝对数）。

