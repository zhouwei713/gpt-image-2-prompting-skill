---
name: gpt-image-2-prompting
description: Write high-quality GPT-Image-2 prompts with strong structure, layout logic, and production-ready visual direction. Use this skill whenever the user asks for image prompts, wants better GPT-Image-2 prompting, wants to upgrade a weak image prompt, asks for prompt templates, wants series-style prompt systems, or needs prompts for posters, UI screens, information graphics, concept art, brand visuals, editorial layouts, or worldbuilding images.
version: 1.0.0
author: Hermes Agent
license: MIT
metadata:
  hermes:
    tags: [image, prompting, gpt-image-2, design, visual-brief, concept-art]
---

# GPT-Image-2 Prompting

This skill turns vague image requests into production-grade GPT-Image-2 prompts.

Core principle:
A strong image prompt should read like a visual brief, not a pile of style words.

## When to use

Trigger this skill whenever the user:
- asks for GPT-Image-2 prompts or better image prompts
- wants to improve a weak prompt
- wants prompts for posters, covers, UI, dashboards, information graphics, packaging, editorial layouts, concept art, or worldbuilding
- asks for prompt templates, batch prompt ideas, themed prompt packs, or reusable prompt systems
- says things like “帮我写提示词”, “优化提示词”, “给我一组出图更高级的 prompt”, “做成系列提示词”

## What this skill optimizes for

1. Strong image type definition
2. Clear visual hierarchy
3. Specific layout and information modules
4. Better conversion of abstract taste words into concrete visual directions
5. Reusable prompt systems instead of one-off lines

## Default workflow

### Step 1: Identify the image type

Always decide the output format first.
Common image types:
- poster
- UI screen / app screen
- dashboard
- infographic
- editorial / magazine cover
- concept art
- design proposal board
- archive sheet / dossier
- map / guide
- packaging / product visual
- storyboard / character sheet

If the user does not specify, infer from context.

### Step 2: Build the prompt around 8 slots

Use this order whenever possible:

1. Image type
2. Core subject
3. Composition / layout
4. Supporting modules
5. Visual tone
6. Material / texture
7. Typography / labeling
8. Aspect ratio

### Step 3: Translate vague taste words

Do not leave words like these unexplained:
- 高级感
- 电影感
- 氛围感
- 科技感
- 杂志感

Translate them into concrete visual instructions.
Examples:
- 高级感 -> restrained layout, limited color palette, clean typography, premium materials, generous negative space
- 电影感 -> low-angle framing, dramatic lighting, foreground/background depth, emotional tension, reflective surfaces
- 科技感 -> glass panels, metal textures, interface modules, cool lighting, precision spacing
- 杂志感 -> editorial hierarchy, strong headline placement, clean grid, short support text, controlled palette

### Step 4: Add visual organization

Most weak prompts only name a subject.
Strong prompts also define the surrounding structure.
Useful supporting modules:
- comment section
- parameter panel
- legend
- annotations
- scale bar
- charts
- ranking list
- route map
- labels
- footer note
- source note
- time axis

### Step 5: Decide whether this should be a single image or a system

If the user wants stronger output, consider turning one prompt into a repeatable system:
- same structure, different era
- same structure, different city
- same structure, different profession
- same structure, different emotion
- same structure, different product line

This usually produces better series content than writing unrelated prompts.

## Prompt writing rules

- Lead with the image type, not the style word
- Prefer concrete layout over generic taste language
- Use style words only after structural decisions are clear
- Include only details that affect the final image
- Keep the prompt dense, but organized
- If the user wants a shareable or viral image, favor contrast, worldbuilding, or system design
- If the user wants a polished commercial image, favor hierarchy, materials, labels, and composition control

## Default response format

When writing prompts for the user, use this structure unless they ask for something else:

### 1. Brief idea
One sentence describing the concept.

### 2. Final prompt
A polished prompt in the user’s language.

### 3. Why this works
2-4 bullets explaining the structural strengths.

### 4. Optional variations
3 short variant directions if useful.

## Chinese default output style

When the user writes in Chinese, default to Chinese output unless they request another language.

Use this delivery structure by default:

### 1. 核心创意
Use 1-2 sentences to explain the visual concept in plain Chinese.

### 2. 完整 Prompt
Give one polished final prompt, usually as one continuous paragraph.

### 3. 为什么这样写
Explain briefly using 2-4 bullets. Focus on:
- 图像类型是否清楚
- 主体和版式是否明确
- 信息模块是否增强了层级
- 抽象审美词是否被翻译成了具体视觉语言

### 4. 可改写方向
Offer 2-3 short variation directions when useful, such as:
- 换时代 / 换城市
- 换职业 / 换情绪
- 换媒介形态（海报、UI、信息图、档案页）
- 换色彩和材质系统

## Chinese phrasing guidance

- Write naturally, like a skilled Chinese visual director giving a brief
- Keep explanations concise and practical
- Avoid jargon overload unless the user clearly wants professional terminology
- Prefer concrete Chinese visual instructions over vague taste words
- If the user asks for a batch of prompts, keep the same output format for each prompt unless a table is clearly better

## Chinese batch mode

When the user asks for multiple prompts at once, default to a structured Chinese batch format.

Use this output structure:

### 分类标题
Name the category first, especially when the batch is large.
Examples:
- 历史世界 × 现代界面
- 信息图 × 情绪表达
- 品牌提案 × 商业视觉
- 世界观档案页
- 城市观察 × 社会情绪

### 每条 Prompt 的默认格式
For each prompt, use:

#### [编号]. [标题]
- 核心创意：用一句话讲清楚这个画面想做什么
- 完整 Prompt：给一条可直接使用的完整 Prompt
- 可替换变量：列 2-4 个最值得替换的变量，方便用户自己扩写

### Batch-size guidance
- 1-5 条：可以保留“为什么这样写”
- 6-20 条：以“核心创意 + 完整 Prompt + 可替换变量”为主，保持紧凑
- 20 条以上：优先按分类分组，减少逐条解释，除非用户明确要求详细拆解

### Default consistency rules
- 同一批内容尽量保持统一结构
- 同一分类优先共享一套视觉逻辑，再替换主题变量
- 如果是做资料包，优先保证可复制、可扩写、可分类整理
- 如果是做灵感清单，可以适当放宽结构，但仍然保留图像类型和版式意识

## Upgrade path for weak prompts

If the user gives a weak prompt, rewrite it by upgrading in this order:
1. clarify image type
2. define subject
3. define composition
4. add modules
5. translate vague taste words
6. add materials / labels / typography
7. choose aspect ratio

## Chinese example response

### 核心创意
做一张“城市失眠指数”主题的信息图海报，把深夜情绪转成可以被观看的数据地图。

### 完整 Prompt
“城市失眠指数”信息图海报，中心是一张俯视夜景地图，按照 22:00、00:00、02:00、04:00 四个时段分层发光，商业区高亮，住宅区以昏黄窗光点阵呈现，四周嵌入咖啡销量、夜间打车热度、音乐播放峰值、社交媒体活跃度四个圆形数据模块，标题像国际杂志专题页，副标题写“谁还醒着，谁在假装睡着”，整体冷静克制，带轻微都市焦虑感，色彩控制在霓虹紫、电蓝、夜黑和少量暖黄，比例 4:5。

### 为什么这样写
- 先定义为“信息图海报”，模型会按专题视觉去组织画面
- 中心地图 + 四周模块，画面层级会更清楚
- “都市焦虑感”被拆成夜景、冷色、高亮区域这些具体视觉指令
- 配色和比例明确后，更容易出成品感

### 可改写方向
- 换成“加班热力图”主题
- 换成“地铁情绪地图”结构
- 换成杂志封面而不是信息图海报

## Chinese batch example

### 历史世界 × 现代界面

#### 1. 唐朝人的外卖 App
- 核心创意：把唐朝日常生活翻译成一张现代外卖首页界面，让历史感和产品感同时成立。
- 完整 Prompt：唐朝人的外卖 App，画面模拟手机外卖首页界面，顶部定位显示“长安·平康坊”，推荐位展示胡饼、炙羊肉、葡萄酿，商家头像采用工笔画掌柜半身像，评分以铜钱图标呈现，底部导航栏完整保留现代产品结构，状态栏显示“大唐信号满格”和“开元二十四年”，整体配色为赭石、石绿、金箔红，字体融合碑刻感标题字与细无衬线，界面像真实产品设计稿，同时带有历史穿越幽默感，比例 9:16。
- 可替换变量：朝代、城市、品类、界面类型

#### 2. 明代人的求职网站首页
- 核心创意：把古代职业体系做成现代招聘平台首页，重点放在职位卡片和筛选逻辑。
- 完整 Prompt：明代人的求职网站首页，历史服饰与现代招聘平台界面融合，主界面有职位推荐“修史官、书院讲郎、船务账房、织造监督、宫廷画师”，筛选条件写“擅诗文、通算学、善骑射、可外派”，人物简历卡使用工笔肖像，薪资单位以俸禄石米表示，整体排版像真实招聘网站首页，比例 16:9。
- 可替换变量：时代、岗位、筛选条件、薪资表达

## Good prompt categories

Use the reference file `references/categories.md` for category patterns and representative examples.
Use `references/templates.md` for reusable fill-in-the-blank templates.

## Common mistakes to avoid

- starting with only style words
- leaving composition undefined
- no information hierarchy
- too many random elements with no focal point
- calling something “高级感” without specifying what creates that feeling
- writing a one-off idea when a reusable prompt system would be better

## Best-practice mindset

The goal is not to produce a merely detailed prompt.
The goal is to produce a prompt with visual intent, structure, and enough control that the output feels designed.
