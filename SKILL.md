---
name: writing-loop-editor
description: "Use when the user is writing, rewriting, expanding, editing, or checking long-form prose: articles, textbook chapters, manuscript sections, commentary, research essays, policy briefs, or explanatory writing. Also use for reader-agent diagnosis, restatement checks, clarity checks, repeated revision loops, or prose that should be clear for humans and easy for AI to revise. Also use when the user says 三层写作Loop, 写作Loop, 自升级编辑, 读者agent, 复述检查, 检查是否清楚, 反复优化, 改文风, 改文章, 把这段改成, 扩写, 写入正文, 教材章节, 长文写作. Do not use for casual chat, simple factual answers, code-only tasks, or short copy edits unrelated to article-style writing. 中文：用于长文写作、改写、扩写、编辑和清晰度检查，尤其是教材章节、书稿、评论文章、研究文章、政策简报和解释性文章；也用于读者 agent 复述、偏差诊断、自升级修改和反复优化。不要用于普通聊天、简单问答、纯代码任务，或与长文写作无关的短句润色。"
metadata:
  short-description: Bilingual long-form writing and reader-agent editing
---

# Writing Loop Editor / 写作 Loop 编辑器

Use this skill to write, rewrite, expand, or edit article-style prose with a clear human-readable and AI-editable style.

使用本 skill 来撰写、改写、扩写或编辑文章式长文。目标是让文本既适合人类阅读，也便于 AI 后续准确修改。

The target style is not imitation of one publication. It combines:

目标文风不是模仿某一家媒体，而是结合以下能力：

- exam-style logical precision from GRE / GMAT / LSAT reading and writing;
- serious journalism's concrete scenes, clear attribution, and readable progression;
- academic or policy brief norms: conclusion first, evidence boundaries, and scan-friendly structure;
- iterative reader-agent checking so the text becomes clearer through repeated restatement, diagnosis, and revision.

- GRE / GMAT / LSAT 式的逻辑清晰度：主旨、证据、推论和限定要分开；
- 严肃新闻写作的具体场景、清楚归因和可读推进；
- 学术简报或政策简报的表达规范：结论靠前、证据边界清楚、结构便于扫读；
- 读者 agent 复述检查：通过复述、诊断和局部改写，让文本在多轮中变清楚。

## When To Use / 什么时候使用

Use this skill for:

- long-form article writing;
- textbook or manuscript chapters;
- research essays and explanatory prose;
- commentary or analysis articles;
- policy or academic briefs;
- rewriting drafts for clearer structure and style;
- checking whether a section is understandable;
- repeated prose optimization through reader-agent review.

适合用于：

- 长文写作；
- 教材章节或书稿章节；
- 研究文章和解释性文章；
- 评论文章或分析文章；
- 政策简报或学术简报；
- 对草稿做结构重写和文风统一；
- 检查某一节是否清楚；
- 通过读者 agent 做多轮复述、诊断和修改。

Do not use it for ordinary chat, simple answers, pure code work, or isolated one-line phrasing unless the user explicitly asks to apply the writing loop.

不要用于普通聊天、简单事实回答、纯代码工作，或孤立的一句话润色，除非用户明确要求使用写作 Loop。

## Core Principles / 核心原则

The writing must satisfy four requirements:

写作必须同时满足四个要求：

1. **Direction / 方向**: the section has a clear narrative and argumentative goal. 每一节都有明确的叙事目标和论证目标。
2. **Paragraph Description / 段内描写**: every paragraph is clear, readable, and performs one main function. 每段清楚、可读，并主要承担一个功能。
3. **Editorial Review / 编辑检查**: after drafting, review from reader, grammar, and professional perspectives. 写完后从普通读者、语法和专业角度检查。
4. **Self-Upgrading Revision / 自升级修改**: use reader agents to restate, diagnose, revise, and restate again until the reader's version and the author's intended meaning mostly match. 用读者 agent 复述、诊断、修改，再复述，直到读者理解和作者意图基本一致。


## Manuscript Chapter Mode / 教材章节模式

Use this mode when writing or revising a long manuscript chapter, textbook chapter, serialized essay, or any article where chapter-level structure matters more than local polish.

当用户正在写长章节、教材、书稿、连载文章，或者文本需要保持全章结构一致时，使用本模式。此时不要只做局部润色，要先判断章节功能、篇幅比例、叙事推进和材料取舍。

### 1. Identify section function before drafting / 写正文前先判断小节功能

Before drafting or expanding a section, identify its function in the chapter: introduction, transition, explanation, example, historical source, task expansion, comparison, compression, or conclusion.

在写作或扩写之前，先判断本节在全章中的功能：它是引入、转向、解释、举例、溯源、展开任务、比较、压缩，还是收束。不要只看局部内容是否正确，要判断它是否服务全章叙事目标。

### 2. Check chapter-level balance / 先看篇幅平衡

Before expanding, check whether the section is proportionate to sibling sections. A valuable section may still need compression if it turns into a standalone survey.

扩写前先检查全章篇幅比例。如果某一节明显超过同级章节，应先压缩或重构，而不是继续增加材料。判断标准不是“内容是否有价值”，而是“它在本章中是否承担相称的功能”。

### 3. Distinguish repetition from functional return / 区分重复和功能性回扣

Repeated concepts are acceptable only when they perform a new function: introduction, transition, historical sourcing, example, qualification, or conclusion.

判断重复时，不只看关键词是否重复，而看每次出现是否增加新功能。若只是换句话说同一判断，应压缩；若承担引入、转向、溯源、例证、限定或收束等不同功能，可以保留，但要显式标出功能差异。

### 4. Use examples by narrative function / 案例必须服务叙事

Do not list examples just to show coverage. Each example must support a clear judgment. If several examples show the same mechanism, keep the clearest one or move the rest to notes.

案例不是越多越好。每个案例必须说明一个明确判断。若多个案例只展示同一机制，应保留最清楚、最能服务本节目标的一个或两个，其余删除或转入注释。

### 5. Explain first, name later / 先通俗解释，再给专业名词

For technical ideas, explain the mechanism in ordinary language before naming the professional term. A term should make the explanation more precise, not replace it.

遇到专业概念时，先给自然语言解释，再给专业名词。专业名词只能让解释更精确，不能替代解释。若读者不懂名词也能理解基本意思，才算合格。

### 6. Use metaphors sparingly and state their limits / 隐喻要克制，并说明边界

A chapter-wide metaphor should usually appear in three places: introduce it near the opening, develop it once in the middle, and recover it in the conclusion. Always explain where the metaphor stops working.

如果一个隐喻要贯穿整章，默认只放三处：开头提出，中段推进一次，结尾回收。不要在每个小节都重复使用，否则隐喻会压过论证。使用隐喻时，必须说明它的适用范围和限制。

### 7. Avoid encyclopedia drift / 避免百科式展开

If a section starts accumulating many algorithms, fields, papers, names, or examples, check whether it is becoming an encyclopedia entry. Keep the main-line material in body prose; move secondary material to notes, comments, or later chapters.

如果一节开始出现大量算法、应用领域、论文名、人物名和横向案例，要检查它是否正在变成百科式展开。教材正文应保留主线材料，其余放入脚注、注释或后续章节。

### 8. Write task types as questions, not algorithm names / 任务类型先写成问题问法

When explaining data science tasks, start from the question the task answers, not from algorithm names. For example: clustering asks “which objects are similar,” anomaly detection asks “which objects deviate,” and association rules ask “which objects often appear together.”

介绍数据科学任务时，优先写它回答什么问题，而不是先列算法名称。比如：聚类回答“哪些对象相似”，异常检测回答“哪些对象偏离常规”，关联规则回答“哪些对象经常一起出现”。

### 9. Mark core sentences in review mode / 审阅模式标出核心句

In review mode, mark the core sentence of each section or paragraph group. If no core sentence can be found, the section likely needs restructuring before polishing.

审阅长文时，可以标出每节或每个段落组的核心句。核心句应说明该段或该节真正承担的判断功能。若找不到核心句，说明该节可能方向不清，需要先重构而不是润色。

### 10. Treat comment callouts as editorial instructions / 将注释块视为编辑指令

When Obsidian callouts such as `[!comment]` appear, treat them as editorial instructions rather than body prose. Read their location, task, requirements, and processing record before editing.

当正文中出现 Obsidian callout `[!comment]` 时，把它视为编辑指令，不视为正文。优先读取其中的位置、任务、要求、处理记录，再决定是否扩写、压缩、查资料或改写。

Suggested format / 推荐格式：

```md
> [!comment] Revision Request / 修改请求
> **Location / 位置**:
> **Task / 任务**: expand / rewrite / add example / fact-check / compress / adjust tone
> **Requirements / 要求**:
> **Processing record / 处理记录**:
```

### 11. Use review colors only when requested or after asking / 审阅颜色仅在触发或询问后使用

Color markup is an optional review mode, not a default writing mode. Use it when the user explicitly asks for colored review marks, revision traces, or core-sentence marking. If colored markup would help but the user did not ask for it, ask briefly whether to enable it before modifying the document.

颜色标记是可选审阅模式，不是默认写作模式。只有当用户明确要求颜色审阅、修改痕迹、核心句标记时才使用。若你判断颜色标记有帮助但用户没有要求，先简短询问是否启用，再修改正文。

When enabled, preserve revision intent with color-coded Markdown or HTML spans:

启用后，用颜色标记不同编辑意图：

- Green / 绿色: rewritten body prose recommended for retention / 重写后建议保留的正文
- Red strikethrough / 红色删除线: content recommended for deletion or non-expansion / 建议删除或不再展开
- Blue / 蓝色: structural note, not body prose / 结构说明，不作为正文
- Orange / 橙色: requires user confirmation / 需要用户确认
- Purple bold / 紫色加粗: core sentence or key judgment / 核心句或主判断

## Layer 1: Direction / 第一层：写作方向

Before writing a section, identify:

写正文前，先明确：

- what the section proves or explains;
- where it moves the reader from and to;
- how it serves the whole article;
- the section's one-sentence core judgment;
- the 3-5 main points;
- the main examples and how each supports the argument;
- how the section connects to the previous and next sections.

- 本节要证明或解释什么；
- 它把读者从哪个理解位置带到哪个理解位置；
- 它如何服务全文主线；
- 本节能否用一句话说出核心判断；
- 3 到 5 个主要要点；
- 主要例子，以及每个例子如何支撑论点；
- 本节如何承接上一节、引出下一节。

If the core judgment cannot be stated in one sentence, do not draft body prose yet.

如果核心判断不能用一句话说清楚，先不要写正文。

Control material by function:

根据材料功能控制展开程度：

- core examples may be expanded; 核心案例可以展开；
- supporting examples should be brief; 辅助案例要简短；
- material that only displays knowledge but does not advance the argument should be cut; 只展示知识、不推进论证的材料应删除；
- useful but rhythm-breaking material should become a note or later section; 有用但打断节奏的材料应放入注释或后文；
- material with unclear relation to the section goal should be withheld. 与本节目标关系不明的材料暂不写入。

Check repetition versus richness globally.

全局检查“重复性”和“丰富性”。

- **Repetition / 重复性**: the text restates the same point with different wording, without adding a new angle, evidence, detail, counterexample, layer, or reader-understanding function.
- **Richness / 丰富性**: the text explores the same point from different angles, such as historical context, concrete scene, mechanism, comparison, counterexample, professional qualification, or reader consequence.

Rules / 判断规则：

- If deleting a passage causes no loss of understanding, it is probably repetition. 删除后读者理解没有损失，通常是重复。
- If deleting a passage removes an angle, evidence type, layer, or qualification, it is probably richness. 删除后少了角度、证据类型、层次或限定，通常是丰富性。
- If two examples show the same mechanism without meaningful scene differences, merge them. 两个例子说明同一机制且场景差异不重要，应合并。
- If two examples show the same claim under different conditions, keep them and clarify the difference. 两个例子展示同一观点在不同条件下的表现，应保留并写清差异。
- If one judgment is repeated several times without progress, keep the clearest version. 一个判断被多次重述但没有推进，保留最清楚的一次。
- If one judgment is developed through different functions, preserve it and organize the functions clearly. 一个判断通过不同功能展开，应保留并整理段落功能。

Do not mistake repetition for depth, and do not cut richness into thinness.

不要把重复误认为深入，也不要把丰富性删成单薄。

## Layer 2: Paragraph-Level Writing / 第二层：段内写作

Each paragraph should do one main thing:

每段原则上只做一件主要事情：

- state a judgment; 提出判断；
- explain a concept; 解释概念；
- develop an example; 展开例子；
- give historical or contextual background; 交代历史或背景；
- compare cases; 做比较；
- transition or summarize. 过渡或总结。

For judgment paragraphs, prefer:

观点段优先使用这个顺序：

1. core judgment; 核心判断；
2. short explanation; 简短解释；
3. necessary example or evidence; 必要例子或证据；
4. return to the point or move it forward. 回到观点，或把观点向前推进。

Keep paragraphs independently understandable, while making their relationship to adjacent paragraphs explicit.

每段单独看要能基本理解，同时要让读者看出它和前后段的关系。

Prefer / 优先使用：

- concrete examples before abstract explanation; 先给具体例子，再做抽象解释；
- clear subjects and verbs; 明确主语和动词；
- short or medium-length sentences; 短句或中等长度句子；
- explicit transitions; 清楚过渡；
- specific nouns and strong verbs; 具体名词和有动作感的动词；
- qualified claims when evidence is limited. 证据有限时降低断言强度。

Reduce / 减少：

- stacked terminology; 术语堆叠；
- stacked adjectives; 形容词堆叠；
- dense abstractions; 密集抽象名词；
- long chains of clauses; 过长从句链；
- repetitive AI-like transitions such as "换句话说", "也就是说", "总的来说", "不仅...还...", unless they are genuinely needed. 机械重复的 AI 式过渡句，除非确实必要。

Track context shifts:

注意语境切换：

- daily-language meaning; 日常语境；
- technical meaning; 技术语境；
- discipline-specific meaning. 学科语境。

When shifting from ordinary language to a professional meaning, tell the reader.

当一个词从日常含义转入专业含义时，要提醒读者。

## Layer 3: Editorial Review / 第三层：编辑检查

After drafting, check from three perspectives.

写完后，从三个角度检查。

### Ordinary Reader / 普通读者

Ask / 检查：

- Can a non-specialist understand the section's main point? 非专业读者能否理解本节主旨？
- Are terms explained before they are needed? 术语是否在需要前解释？
- Are examples concrete enough? 例子是否足够具体？
- Does the section start from an accessible point? 开头是否从读者可进入的位置开始？
- Do paragraphs visibly progress? 段落之间是否有可见推进？
- Is there any sudden jump into professional judgment? 是否突然跳入专业判断？
- Are there too many unexplained abstractions? 是否有太多未解释的抽象概念？

### Grammar Police / 语法警察

Ask / 检查：

- Are sentences smooth? 句子是否顺畅？
- Is the subject clear? 主语是否清楚？
- Are verb-object pairings natural? 动宾搭配是否自然？
- Are parallel items the same kind of thing? 并列项是否属于同一类？
- Are long sentences split when needed? 长句是否需要拆开？
- Is punctuation reasonable? 标点是否合理？
- Are pronouns such as "it", "this", "these", "这个", "这些" clear? 代词指代是否清楚？
- Are there redundancies, awkward phrasing, or unwanted chatty residue? 是否有冗余、别扭表达或聊天残留？

### Professional Reviewer / 专业审稿人

Ask / 检查：

- Is the logic coherent? 逻辑是否连贯？
- Are concepts accurate? 概念是否准确？
- Are technical terms appropriate? 术语是否合适？
- Are factual claims reliable? 事实判断是否可靠？
- Does the evidence support the conclusion? 证据是否支撑结论？
- Is any analogy overextended? 类比是否过度延伸？
- Does any conclusion exceed the evidence? 结论是否超出证据？
- Should the claim be softened with "usually", "often", "can be understood as", or a note? 是否需要用“通常”“往往”“可以理解为”等方式降低强度？

If uncertain, lower the claim's strength, add a qualification, add a note, or leave the claim out of body prose.

如果不确定，降低判断强度，补充限定，放入注释，或暂不写入正文。

## Layer 4: Self-Upgrading Reader-Agent Revision / 第四层：自升级读者修改

Use this mode when the user asks whether a text is clear, asks for repeated optimization, or asks to rewrite a passage in a specific direction.

当用户要求检查是否清楚、反复优化，或把一段文字改成某种方向时，使用这一模式。

The loop is:

基本流程：

1. read the original; 阅读原文；
2. simulate reader agents; 模拟不同读者 agent；
3. ask each reader agent to restate what it understood; 让每个读者复述自己理解到的内容；
4. compare the restatement with the author's intended meaning; 比较读者复述和作者意图；
5. diagnose the source of divergence; 诊断偏差来源；
6. revise the smallest useful unit; 修改最小有效单位；
7. restate again. 再次复述检查。

Do not jump straight into polishing. Restatement exposes misunderstanding that polishing may hide.

不要直接润色。复述能暴露误解，而润色可能掩盖误解。

### Reader Agents / 读者 Agent

Use at least three agents:

至少使用三类读者：

- **ordinary reader agent / 普通读者 agent**: has no systematic professional background and relies on the text alone. 没有系统专业背景，只依靠文本理解。
- **semi-professional reader agent / 半专业读者 agent**: knows some terms and field context but not the full theory or method. 知道一些术语和背景，但不了解完整理论或方法。
- **professional reader agent / 专业读者 agent**: checks concepts, logic, evidence, and professional expression. 检查概念、逻辑、证据和专业表达。

Add when useful:

必要时增加：

- **writing editor agent / 写作编辑 agent**: checks paragraph rhythm, sentence order, and clarity. 检查段落节奏、句序和清晰度。
- **skeptical reader agent / 怀疑型读者 agent**: looks for leaps, overclaims, and weak evidence. 检查跳跃、过度断言和弱证据。
- **beginner agent / 初学者 agent**: checks whether examples are concrete and terms are explained. 检查例子是否具体、术语是否解释。

### 80 Percent Understanding Threshold / 80% 理解阈值

Reader agents should clearly recover at least about 80 percent of the intended meaning.

读者 agent 至少要能恢复作者原意的大约 80%。

Check three kinds of consistency:

检查三类一致性：

- **logical consistency / 逻辑一致性**: the reader recovers the main claim, reasoning order, and paragraph relationship. 读者能复述主论点、推理顺序和段落关系。
- **detail consistency / 细节一致性**: the reader does not miss key facts, examples, qualifications, or concept distinctions. 读者没有漏掉关键事实、例子、限定和概念差异。
- **tone consistency / 语气一致性**: the reader does not mistake a cautious claim for a strong assertion, or a side point for the main claim. 读者不会把谨慎判断误读成强断言，也不会把支线当主线。

If the reader only understands the broad topic but cannot explain the reasoning path, the passage is not clear enough.

如果读者只知道大概主题，却说不清推理路径，文本还不够清楚。

### Diagnosis Before Revision / 先诊断，再修改

When the restatement diverges from the intended meaning, identify the problem type before rewriting.

当读者复述偏离作者意图时，先判断问题类型，再改写。

Common problems / 常见问题：

- the core judgment appears too late; 核心判断出现太晚；
- one paragraph does too many things; 一段承担太多功能；
- a term shifts from ordinary to professional context without warning; 术语从日常语境跳到专业语境但没有提醒；
- an example does not clearly serve a point; 例子没有清楚服务观点；
- background information buries the main line; 背景信息压住主线；
- sentence subjects or actions are unclear; 句子主语或动作不清；
- transitions are missing, so the reader guesses the relation; 缺少过渡，读者只能猜段落关系；
- tone is stronger than the evidence; 语气强于证据；
- important qualifications are hidden; 关键限定被藏起来；
- paragraph order does not match the reader's understanding path. 段落顺序不符合读者理解路径。

### Revision Order / 修改顺序

Revise in this order:

按这个顺序修改：

1. structure: paragraph order, paragraph function, reasoning path; 结构：段落顺序、段落功能、推理路径；
2. judgment: move core sentences earlier and clarify conclusions; 判断：提前核心句，明确结论；
3. examples: make examples concrete and tie them to claims; 例子：让例子具体，并和观点连接；
4. sentences: fix long sentences, pairings, pronouns, and transitions; 句子：处理长句、搭配、指代和过渡；
5. style: adjust rhythm, repetition, tone, and word choice. 文风：调整节奏、重复、语气和词语。

Many sentence problems come from structural problems, so avoid word-level tinkering too early.

很多句子问题来自结构问题，所以不要过早停留在字词层面。

## Execution Modes / 执行模式

### If Asked To Draft / 如果用户要求起草

First provide a short direction note:

先给简短写作方向说明：

- section goal; 本节目标；
- core judgment; 核心判断；
- outline; 提纲；
- examples; 例子；
- connection to previous and next sections. 与前后文的关系。

Then write body prose.

然后再写正文。

### If Asked To Rewrite / 如果用户要求改写

For explicit modification tasks such as "change this passage into X", "把这段改成...", or "rewrite this in this direction", front-load the reader-agent loop before rewriting.

对“把这段改成……”“按这个方向重写”等明确改写任务，先做读者 agent 复述和诊断，再改写。

First:

先做：

- have reader agents review the original passage; 让读者 agent 阅读原文；
- restate the user's target version or requested direction; 复述用户要求的目标方向；
- compare the original, the target, and the likely reader understanding; 比较原文、目标方向和读者可能理解；
- diagnose what must change. 诊断必须修改的地方。

Briefly diagnose:

简短说明：

- current paragraph function; 当前段落功能；
- where the structure or meaning is unclear; 结构或意思哪里不清楚；
- what will be changed. 将要修改什么。

Then rewrite.

然后再改写。

### If Asked To Check Clarity / 如果用户要求检查是否清楚

Use reader-agent restatement first. Do not directly polish.

先用读者 agent 复述，不要直接润色。

Output:

输出：

- ordinary reader restatement; 普通读者复述；
- semi-professional reader restatement; 半专业读者复述；
- professional reader concerns; 专业读者问题；
- divergence diagnosis; 偏差诊断；
- concrete revision plan or revised text if requested. 如用户要求，给出具体修改计划或改写文本。

### If Asked To Repeatedly Optimize / 如果用户要求反复优化

Run at least one full loop:

至少运行一轮完整 Loop：

1. restatement; 复述；
2. diagnosis; 诊断；
3. localized revision; 局部修改；
4. second restatement; 第二次复述；
5. stop only when logic, details, and tone mostly match the intended meaning. 只有当逻辑、细节和语气基本贴合原意时才停止。

## Output Rules / 输出规则

- If the user asks for an outline, do not write body prose yet. 如果用户要提纲，先不要写正文。
- If the user asks to write into body prose, briefly state the direction and then write. 如果用户要求写成正文，先简短说明方向，再写正文。
- If the user asks to change style, prioritize paragraph function, sentence rhythm, and reader understanding. 如果用户要求改文风，优先处理段落功能、句子节奏和读者理解。
- If the user says the draft is wrong, diagnose the divergence before continuing to expand. 如果用户说草稿不对，先诊断偏差，再继续扩写。
- Keep comments separate from body prose when the user asks for comments or review notes. 用户要求评论或审阅意见时，把评论和正文分开。
