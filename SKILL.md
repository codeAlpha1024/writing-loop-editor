---
name: writing-loop-editor
description: Use when the user is writing, rewriting, expanding, editing, or checking a long-form article, textbook chapter, commentary, research essay, policy brief, or explanatory prose. Also use when the user says 三层写作Loop, 写作Loop, 自升级编辑, 读者agent, 复述检查, 检查是否清楚, 反复优化, 改文风, 改文章, 把这段改成, 扩写, 写入正文, 教材章节, 长文写作, or asks for prose that is clear for humans and easy for AI to revise. Do not use for casual chat, simple factual answers, code-only tasks, or short copy edits unrelated to article-style writing.
metadata:
  short-description: Clear article writing and iterative reader-agent editing
---

# Writing Loop Editor

Use this skill to write, rewrite, expand, or edit article-style prose with a clear human-readable and AI-editable style.

The target style is not imitation of one publication. It combines:

- exam-style logical precision from GRE / GMAT / LSAT reading and writing;
- serious journalism's concrete scenes, clear attribution, and readable progression;
- academic or policy brief norms: conclusion first, evidence boundaries, and scan-friendly structure;
- iterative reader-agent checking so the text becomes clearer through repeated restatement, diagnosis, and revision.

## When To Use

Use this skill for:

- long-form article writing;
- textbook or manuscript chapters;
- research essays and explanatory prose;
- commentary or analysis articles;
- policy or academic briefs;
- rewriting drafts for clearer structure and style;
- checking whether a section is understandable;
- repeated prose optimization through reader-agent review.

Do not use it for ordinary chat, simple answers, pure code work, or isolated one-line phrasing unless the user explicitly asks to apply the writing loop.

## Core Principles

The writing must satisfy four requirements:

1. **Direction**: the section has a clear narrative and argumentative goal.
2. **Paragraph Description**: every paragraph is clear, readable, and performs one main function.
3. **Editorial Review**: after drafting, review from reader, grammar, and professional perspectives.
4. **Self-Upgrading Revision**: use reader agents to restate, diagnose, revise, and restate again until the reader's version and the author's intended meaning mostly match.

## Layer 1: Direction

Before writing a section, identify:

- what the section proves or explains;
- where it moves the reader from and to;
- how it serves the whole article;
- the section's one-sentence core judgment;
- the 3-5 main points;
- the main examples and how each supports the argument;
- how the section connects to the previous and next sections.

If the core judgment cannot be stated in one sentence, do not draft body prose yet.

Control material by function:

- core examples may be expanded;
- supporting examples should be brief;
- material that only displays knowledge but does not advance the argument should be cut;
- useful but rhythm-breaking material should become a note or later section;
- material with unclear relation to the section goal should be withheld.

Check repetition versus richness globally.

Repetition and richness can both circle the same claim, but they are different:

- **repetition**: the text restates the same point with different wording, without adding a new angle, evidence, detail, counterexample, layer, or reader-understanding function;
- **richness**: the text explores the same point from different angles, such as historical context, concrete scene, mechanism, comparison, counterexample, professional qualification, or reader consequence.

Rules:

- If deleting a passage causes no loss of understanding, it is probably repetition.
- If deleting a passage removes an angle, evidence type, layer, or qualification, it is probably richness.
- If two examples show the same mechanism without meaningful scene differences, merge them.
- If two examples show the same claim under different conditions, keep them and clarify the difference.
- If one judgment is repeated several times without progress, keep the clearest version.
- If one judgment is developed through different functions, preserve it and organize the functions clearly.

Do not mistake repetition for depth, and do not cut richness into thinness.

## Layer 2: Paragraph-Level Writing

Each paragraph should do one main thing:

- state a judgment;
- explain a concept;
- develop an example;
- give historical or contextual background;
- compare cases;
- transition or summarize.

For judgment paragraphs, prefer:

1. core judgment;
2. short explanation;
3. necessary example or evidence;
4. return to the point or move it forward.

Keep paragraphs independently understandable, while making their relationship to adjacent paragraphs explicit.

Prefer:

- concrete examples before abstract explanation;
- clear subjects and verbs;
- short or medium-length sentences;
- explicit transitions;
- specific nouns and strong verbs;
- qualified claims when evidence is limited.

Reduce:

- stacked terminology;
- stacked adjectives;
- dense abstractions;
- long chains of clauses;
- repetitive AI-like transitions such as "换句话说", "也就是说", "总的来说", "不仅...还...", unless they are genuinely needed.

Track context shifts:

- daily-language meaning;
- technical meaning;
- discipline-specific meaning.

When shifting from ordinary language to a professional meaning, tell the reader.

## Layer 3: Editorial Review

After drafting, check from three perspectives.

### Ordinary Reader

Ask:

- Can a non-specialist understand the section's main point?
- Are terms explained before they are needed?
- Are examples concrete enough?
- Does the section start from an accessible point?
- Do paragraphs visibly progress?
- Is there any sudden jump into professional judgment?
- Are there too many unexplained abstractions?

### Grammar Police

Ask:

- Are sentences smooth?
- Is the subject clear?
- Are verb-object pairings natural?
- Are parallel items the same kind of thing?
- Are long sentences split when needed?
- Is punctuation reasonable?
- Are pronouns such as "it", "this", "these", "这个", "这些" clear?
- Are there redundancies, awkward phrasing, or unwanted chatty residue?

### Professional Reviewer

Ask:

- Is the logic coherent?
- Are concepts accurate?
- Are technical terms appropriate?
- Are factual claims reliable?
- Does the evidence support the conclusion?
- Is any analogy overextended?
- Does any conclusion exceed the evidence?
- Should the claim be softened with "usually", "often", "can be understood as", or a note?

If uncertain, lower the claim's strength, add a qualification, add a note, or leave the claim out of body prose.

## Layer 4: Self-Upgrading Reader-Agent Revision

This is the main editing mode when the user asks whether a text is clear or asks for repeated optimization.

The loop is:

1. read the original;
2. simulate reader agents;
3. ask each reader agent to restate what it understood;
4. compare the restatement with the author's intended meaning;
5. diagnose the source of divergence;
6. revise the smallest useful unit;
7. restate again.

Do not jump straight into polishing. Restatement exposes misunderstanding that polishing may hide.

### Reader Agents

Use at least three agents:

- **ordinary reader agent**: has no systematic professional background and relies on the text alone;
- **semi-professional reader agent**: knows some terms and field context but not the full theory or method;
- **professional reader agent**: checks concepts, logic, evidence, and professional expression.

Add when useful:

- **writing editor agent**: checks paragraph rhythm, sentence order, and clarity;
- **skeptical reader agent**: looks for leaps, overclaims, and weak evidence;
- **beginner agent**: checks whether examples are concrete and terms are explained.

### 80 Percent Understanding Threshold

The minimum standard is that reader agents can clearly recover at least about 80 percent of the original meaning.

Treat this as three kinds of consistency:

- **logical consistency**: the reader recovers the main claim, reasoning order, and paragraph relationship;
- **detail consistency**: the reader does not miss key facts, examples, qualifications, or concept distinctions;
- **tone consistency**: the reader does not mistake a cautious claim for a strong assertion, or a side point for the main claim.

If the reader only understands the broad topic but cannot explain the reasoning path, the passage is not clear enough.

### Diagnosis Before Revision

When the restatement diverges from the intended meaning, identify the problem type before rewriting.

Common problems:

- the core judgment appears too late;
- one paragraph does too many things;
- a term shifts from ordinary to professional context without warning;
- an example does not clearly serve a point;
- background information buries the main line;
- sentence subjects or actions are unclear;
- transitions are missing, so the reader guesses the relation;
- tone is stronger than the evidence;
- important qualifications are hidden;
- paragraph order does not match the reader's understanding path.

### Revision Order

Revise in this order:

1. structure: paragraph order, paragraph function, reasoning path;
2. judgment: move core sentences earlier and clarify conclusions;
3. examples: make examples concrete and tie them to claims;
4. sentences: fix long sentences, pairings, pronouns, and transitions;
5. style: adjust rhythm, repetition, tone, and word choice.

Many sentence problems come from structural problems, so avoid word-level tinkering too early.

## Execution Modes

### If Asked To Draft

First provide a short direction note:

- section goal;
- core judgment;
- outline;
- examples;
- connection to previous and next sections.

Then write body prose.

### If Asked To Rewrite

For explicit modification tasks such as "change this passage into X", "把这段改成...", or "rewrite this in this direction", front-load the reader-agent loop before rewriting.

First:

- have reader agents review the original passage;
- restate the user's target version or requested direction;
- compare the original, the target, and the likely reader understanding;
- diagnose what must change.

Briefly diagnose:

- current paragraph function;
- where the structure or meaning is unclear;
- what will be changed.

Then rewrite.

### If Asked To Check Clarity

Use reader-agent restatement first. Do not directly polish.

Output:

- ordinary reader restatement;
- semi-professional reader restatement;
- professional reader concerns;
- divergence diagnosis;
- concrete revision plan or revised text if requested.

### If Asked To Repeatedly Optimize

Run at least one full loop:

1. restatement;
2. diagnosis;
3. localized revision;
4. second restatement;
5. stop only when logic, details, and tone mostly match the intended meaning.

## Output Rules

- If the user asks for an outline, do not write body prose yet.
- If the user asks to write into body prose, briefly state the direction and then write.
- If the user asks to change style, prioritize paragraph function, sentence rhythm, and reader understanding.
- If the user says the draft is wrong, diagnose the divergence before continuing to expand.
- Keep comments separate from body prose when the user asks for comments or review notes.
