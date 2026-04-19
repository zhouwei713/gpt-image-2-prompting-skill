# GPT-Image-2 Prompting Skill

中文 | [English](#english)

A high-quality prompting skill for GPT-Image-2 that turns vague image ideas into production-grade prompts with clear structure, visual hierarchy, and reusable prompt systems.

一个面向 GPT-Image-2 的高质量提示词 Skill。
它的目标不是“多写几个风格词”，而是把模糊的图像想法升级成更像视觉总监 brief 的生产级 Prompt。

## Highlights

- Structured prompting instead of keyword piles
- Better control over layout, hierarchy, modules, materials, and aspect ratio
- Strong Chinese-first output mode
- Batch prompt generation for prompt packs and content libraries
- Reusable templates, categories, and examples included

这个 Skill 特别适合下面这些场景：
- 你想为 GPT-Image-2 写出更高级、更稳定的提示词
- 你只有一个模糊概念，想把它变成真正可用的图像 Prompt
- 你想批量生成一组风格统一、结构稳定的 Prompt
- 你在做海报、UI、信息图、杂志封面、概念图、品牌视觉、世界观设定图
- 你想把“高级感、电影感、科技感”这类空泛描述，翻译成真正可执行的视觉语言

---

## Quick Start

If you want to improve this repository, see [CONTRIBUTING.md](CONTRIBUTING.md).


### Hermes

1. Put this skill folder into your Hermes skills directory
2. Ensure Hermes can discover the skill
3. Ask Hermes things like:
   - 帮我写一个 GPT-Image-2 Prompt
   - 优化一下这个图片 Prompt
   - 给我 10 条未来城市风 Prompt
   - 把这个模糊想法变成可直接用的 Prompt

### Expected output

For single prompts, the default Chinese structure is:
- 核心创意
- 完整 Prompt
- 为什么这样写
- 可改写方向

For batch prompts, the default structure is:
- 分类标题
- 标题
- 核心创意
- 完整 Prompt
- 可替换变量

---

## 中文

### 这个 Skill 能做什么

这个 Skill 的核心能力有 5 个：

1. 把模糊需求变成结构化 Prompt
2. 自动补全图像类型、构图、信息模块、材质、色彩、比例这些关键要素
3. 把“高级感 / 电影感 / 科技感 / 杂志感”翻译成更具体的视觉指令
4. 让单条 Prompt 更像“设计稿说明”而不是“关键词堆砌”
5. 支持单条输出和批量输出两种模式

简单说，它不是“灵感词库”，而是一套 Prompt 生成方法。

---

### 这个 Skill 适合哪些图像类型

它最适合下面这些图像任务：

- 海报（Poster）
- UI 页面 / App 页面
- Dashboard / 数据界面
- 信息图（Infographic）
- 杂志封面 / Editorial 视觉
- 概念图（Concept Art）
- 品牌提案图 / 包装提案图
- 档案页 / Dossier / 世界观设定页
- 地图 / 导览图 / 路线图
- 产品视觉 / 包装视觉
- 分镜板 / 角色设定页

如果用户没有明确说图像类型，Skill 会优先根据上下文推断。

---

### 它和普通 Prompt 写法的区别

普通写法通常像这样：
- 帮我生成一张未来城市风海报
- 帮我做一个科技感 UI
- 帮我做一张高级感图片

这种写法也能出图，但很容易飘。
因为模型需要自己猜：
- 这到底是什么类型的图
- 主体是什么
- 版式怎么排
- 什么地方该突出
- 什么地方该留白

这个 Skill 的做法不一样。
它会优先把 Prompt 组织成下面这 8 个槽位：

1. 图像类型
2. 核心主体
3. 构图 / 版式
4. 辅助模块
5. 视觉气质
6. 材质 / 纹理
7. 标题 / 标签 / 文字系统
8. 画幅比例

也就是说，它关注的是“画面组织能力”，不只是风格描述。

---

### 这个 Skill 的默认工作流

#### Step 1：先定图像类型
Skill 会先判断这是海报、UI、信息图、品牌提案还是世界观档案页。

#### Step 2：再搭 Prompt 骨架
Skill 默认使用 8 槽位结构来补足 Prompt。

#### Step 3：翻译空泛审美词
比如：
- 高级感 -> 留白、克制排版、少量配色、玻璃/金属材质、干净字体
- 电影感 -> 低机位、情绪灯光、前后景层次、反光地面、画面张力
- 科技感 -> 玻璃面板、金属结构、界面模块、冷色照明、精密 spacing
- 杂志感 -> 标题层级、编辑排版、短文案、网格感、留白控制

#### Step 4：增加信息层级
Skill 会优先补充这些常见模块：
- 评论区
- 参数栏
- 图例
- 注释标签
- 比例尺
- 图表
- 排行榜
- 路线图
- 时间轴
- 页脚说明

#### Step 5：判断要不要做成“系统”
很多情况下，一条 Prompt 不如一套 Prompt 系统好用。
比如：
- 同一结构，换时代
- 同一结构，换城市
- 同一结构，换职业
- 同一结构，换情绪
- 同一结构，换产品线

---

### 中文输出能力

这个 Skill 专门增强过中文输出。
如果用户用中文提问，它默认会用中文交付，并且优先按照更适合中文用户理解的方式输出。

#### 单条 Prompt 默认格式

1. 核心创意
2. 完整 Prompt
3. 为什么这样写
4. 可改写方向

#### 批量 Prompt 默认格式

当用户一次要多条 Prompt 时，Skill 会自动切换到“中文批量模式”。

默认结构：
- 分类标题
- 每条 Prompt 的标题
- 核心创意
- 完整 Prompt
- 可替换变量

它还会根据数量自动调整细节密度：
- 1-5 条：可以保留“为什么这样写”
- 6-20 条：以“核心创意 + 完整 Prompt + 可替换变量”为主
- 20 条以上：优先分组，减少逐条解释，方便做资料包

---

### 这个 Skill 解决的典型问题

它特别适合解决下面这些问题：

- Prompt 太短，信息不够，出图随机
- Prompt 只有风格词，没有结构
- 用户说了“高级感”，但没有可执行的视觉指令
- 批量写 Prompt 时，风格前后不统一
- 需要做海报、信息图、品牌提案时，不知道该怎么组织画面
- 想把一个模糊概念写成真正有成品感的 Prompt

---

### 内置参考内容

这个 Skill 自带 3 份参考文件：

#### 1. `references/templates.md`
可复用 Prompt 模板库，适合快速扩写。
包括：
- 历史世界 × 现代界面
- 情绪 × 数据可视化海报
- 人物/职业 × 静物叙事
- 空间 × 设计提案图
- 世界观 × 档案页
- 日常事件 × 电影海报
- 年鉴封面 × 总结图

#### 2. `references/categories.md`
把整套 Prompt 方法归纳成 10 个大类，方便快速匹配任务类型。

#### 3. `references/examples.md`
代表性示例集合，适合直接借鉴或做结构映射。

---

### 目录结构

```text
gpt-image-2-prompting/
├── SKILL.md
├── README.md
└── references/
    ├── templates.md
    ├── categories.md
    └── examples.md
```

---

### 使用示例

#### 示例 1：用户只有一个很模糊的需求
用户：
“帮我写一个未来城市风的图片提示词。”

Skill 会把它升级成更完整的输出，例如：
- 核心创意：未来城市夜景概念海报，重点放在立体交通和发光建筑系统
- 完整 Prompt：一条包含主体、构图、信息层级、材质、色彩和比例的完整 Prompt
- 为什么这样写：解释为什么这个结构更容易出精品
- 可改写方向：清晨版、交通中枢版、俯视地图版

#### 示例 2：用户想批量写 Prompt
用户：
“给我 20 条未来城市风 Prompt。”

Skill 会优先：
- 先按类别分组
- 每条保留“核心创意 + 完整 Prompt + 可替换变量”
- 控制整体结构统一，方便整理成资料包

#### 示例 3：用户想优化已有 Prompt
用户：
“我现在这条 Prompt 太普通了，帮我优化一下。”

Skill 会按这个顺序改写：
1. 定图像类型
2. 定主体
3. 定构图
4. 补信息模块
5. 翻译空泛审美词
6. 补材质 / 标签 / 字体
7. 定比例

---

### 最适合谁

这个 Skill 最适合：
- 经常写图片 Prompt 的人
- 做内容、做封面、做海报的人
- 做概念图、世界观设定图的人
- 做品牌视觉、提案图、信息图的人
- 想系统学 Prompt，而不是只想抄几句的人

---

### 安装 / 使用方式

如果你在 Hermes 里使用这个 Skill：

1. 把技能目录放到你的 skills 目录下
2. 确保 Hermes 可以发现该 Skill
3. 在提到图像 Prompt 相关任务时，让 Hermes 调用它

例如你可以直接这样说：
- 帮我写一个 GPT-Image-2 Prompt
- 优化一下这个图片 Prompt
- 做一组海报风 Prompt
- 按资料包结构给我 20 条 Prompt
- 把这个模糊想法变成可直接用的 Prompt

---

### 设计原则

这个 Skill 的核心设计原则只有一句话：

> A strong image prompt should read like a visual brief, not a pile of style words.

翻成中文就是：
一条好 Prompt，读起来应该像视觉 brief，而不是一串风格词。

---

### 许可

本 Skill 当前默认采用仓库作者自行指定的开源或共享方式。
如果你准备公开发布到 GitHub，建议在仓库中补充明确的 LICENSE 文件。

---

## English

### What this skill does

This is a high-quality prompting skill for GPT-Image-2.
Its goal is not to generate random style-heavy prompts, but to turn vague image ideas into production-grade prompts that read like visual briefs.

It is especially useful when you want to:
- write better GPT-Image-2 prompts
- upgrade a weak or overly generic prompt
- generate batches of prompts with consistent quality
- create prompts for posters, UI screens, infographics, editorial layouts, concept art, brand visuals, or worldbuilding images
- translate vague taste words like “premium”, “cinematic”, or “techy” into concrete visual instructions

---

### Core capabilities

This skill is designed to do five things well:

1. Turn vague requests into structured prompts
2. Automatically complete key missing pieces such as image type, composition, support modules, materials, palette, and aspect ratio
3. Translate abstract aesthetic words into practical visual language
4. Produce prompts that feel closer to design briefs than keyword piles
5. Support both single-prompt and batch-prompt workflows

In short, this is not just a prompt collection. It is a prompting method.

---

### Best-fit image types

This skill works best for:
- posters
- UI / app screens
- dashboards
- infographics
- editorial layouts / magazine covers
- concept art
- design proposal boards
- dossier / archive sheets
- maps / guides
- packaging / product visuals
- storyboards / character sheets

If the user does not explicitly specify the format, the skill infers it from context.

---

### How it differs from ordinary prompting

A typical weak prompt looks like this:
- create a futuristic city poster
- make a tech-style UI
- generate a premium image

That can still produce an image, but the result often drifts because the model has to guess:
- what kind of image this actually is
- what the focal point should be
- how the layout should be structured
- what should be prominent and what should recede

This skill uses a more controlled structure.
It builds prompts around 8 slots:

1. image type
2. core subject
3. composition / layout
4. supporting modules
5. visual tone
6. materials / textures
7. typography / labels
8. aspect ratio

That means it optimizes for visual organization, not just style naming.

---

### Default workflow

#### Step 1: Define the image type
The skill first decides whether the request is a poster, interface, infographic, editorial cover, proposal board, or dossier-like image.

#### Step 2: Build the prompt skeleton
It uses the 8-slot structure above to complete the prompt.

#### Step 3: Translate vague taste language
Examples:
- premium -> restrained layout, limited palette, clean typography, premium materials, negative space
- cinematic -> low-angle framing, dramatic lighting, foreground/background depth, reflective surfaces, emotional tension
- futuristic -> interface modules, glass surfaces, metal textures, cool light, precision spacing
- editorial -> clear headline hierarchy, grid logic, support text, layout control

#### Step 4: Add information hierarchy
The skill often adds support modules such as:
- comments
- parameter bars
- legends
- annotation labels
- charts
- timelines
- rankings
- maps
- footer notes

#### Step 5: Decide whether the task should become a prompt system
In many cases, a reusable system is more valuable than a single prompt.
For example:
- same structure, different era
- same structure, different city
- same structure, different profession
- same structure, different emotion
- same structure, different product line

---

### Chinese-first output support

This skill has been specially tuned for Chinese users.
When the user asks in Chinese, it defaults to Chinese output unless another language is explicitly requested.

#### Default single-prompt delivery
- Core idea
- Final prompt
- Why it works
- Variation directions

#### Default batch-prompt delivery
When the user asks for multiple prompts, the skill switches into a structured Chinese batch mode.
It groups prompts by category and uses a stable format for each item.

This makes it suitable for:
- prompt packs
- fan handouts
- content libraries
- internal visual ideation docs

---

### Included reference files

This skill ships with three reference files:

#### `references/templates.md`
Reusable prompt templates for fast expansion.
Includes patterns such as:
- historical world × modern interface
- emotion × infographic poster
- subject × editorial still life
- space × proposal board
- worldbuilding × dossier page
- daily life × cinematic poster
- annual archive × cover system

#### `references/categories.md`
A category map that compresses the full prompt library into 10 reusable archetypes.

#### `references/examples.md`
Representative example prompts that can be adapted directly or used as structural references.

---

### Directory structure

```text
gpt-image-2-prompting/
├── SKILL.md
├── README.md
└── references/
    ├── templates.md
    ├── categories.md
    └── examples.md
```

---

### Example use cases

#### Example 1: The user only has a vague idea
User:
“Write a future city style image prompt.”

The skill will expand that into:
- a clear concept statement
- a full production-grade prompt
- a short explanation of why the structure works
- 2-3 variation directions

#### Example 2: The user wants a batch of prompts
User:
“Give me 20 future-city prompts.”

The skill will typically:
- group them by category
- keep the structure stable across prompts
- include core idea + final prompt + replaceable variables
- make the output easier to turn into a prompt pack

#### Example 3: The user wants prompt optimization
User:
“My current prompt feels too weak. Improve it.”

The skill upgrades it in this order:
1. clarify image type
2. define subject
3. define composition
4. add modules
5. translate vague taste words
6. add materials / labels / typography
7. choose aspect ratio

---

### Who this skill is for

This skill is a good fit for:
- people who frequently write image prompts
- content creators making covers and visual assets
- concept artists and worldbuilders
- designers creating posters, systems, or proposal visuals
- anyone who wants to learn prompting as a method, not just copy random prompts

---

### Installation / usage

If you use this skill inside Hermes:

1. place the skill folder inside your skills directory
2. ensure Hermes can discover the skill
3. invoke it whenever the task involves image prompting

Typical requests:
- write a GPT-Image-2 prompt for me
- improve this image prompt
- create a poster prompt pack
- give me 20 prompts in a structured prompt-pack style
- turn this vague idea into a usable prompt

---

### Design principle

The skill is built around one sentence:

> A strong image prompt should read like a visual brief, not a pile of style words.

That principle drives the entire structure of the skill.

---

### License

This skill currently uses whatever licensing model the repository author chooses.
If you plan to publish it on GitHub, it is strongly recommended to add a clear LICENSE file to the repository.
