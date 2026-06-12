# Writing Loop Editor / 写作 Loop 编辑器

Writing Loop Editor is a Codex skill for long-form prose writing and revision. It is designed for article-style Chinese or English writing where structure, reader understanding, evidence boundaries, and iterative revision matter.

写作 Loop 编辑器是一个用于长文写作与修改的 Codex skill。它适合处理中英文文章式写作，重点关注结构清楚、读者能理解、证据边界明确，以及通过多轮复述和诊断不断改进文本。

## Use Cases / 适用场景

Use it for:

- textbook or manuscript chapters;
- research essays and explanatory prose;
- commentary, analysis, policy briefs, or academic-style drafts;
- rewriting drafts for clearer structure and style;
- reader-agent restatement, clarity checks, and repeated revision loops.

适合用于：

- 教材章节、书稿章节；
- 研究文章、解释性长文；
- 评论文章、分析文章、政策简报、学术风格草稿；
- 对已有草稿做结构重写和文风统一；
- 使用读者 agent 复述、检查清晰度，并进行多轮修改。

Do not use it for ordinary chat, simple factual answers, code-only tasks, or isolated one-line copy edits unless you explicitly want to apply the writing loop.

不适合普通聊天、简单事实问答、纯代码任务，或孤立的一句话润色，除非你明确要求使用写作 Loop。

## The Three Writing Layers / 三层写作

The skill is organized around three writing layers:

1. **Direction / 写作方向层**: define what the section is trying to prove or explain, how it moves the reader, which examples matter, and how the section connects to the larger argument.
2. **Paragraph-Level Writing / 段内描写层**: make each paragraph clear, readable, and functionally focused, with concrete examples, explicit transitions, and fewer empty abstractions.
3. **Editorial Review / 编辑视角层**: review the draft from ordinary-reader, grammar, and professional perspectives, checking clarity, sentence flow, logic, evidence, and claim strength.

这个 skill 的基础结构是三层写作：

1. **写作方向层**：先判断这一节要证明或解释什么、把读者带到哪里、哪些例子真正服务主线，以及本节和全文结构的关系。
2. **段内描写层**：让每一段清楚、可读、功能明确，优先使用具体例子、清楚过渡和低噪音语言，减少空泛抽象。
3. **编辑视角层**：从普通读者、语法和专业审稿三个角度检查文本，确认读者是否看得懂、句子是否顺、逻辑和证据是否站得住。

## Core Loop: Revision / 核心部件：修改 Loop

The most important part of this skill is not one-shot drafting. It is the revision loop.

The loop is:

1. reader agents restate what they understood;
2. the editor compares that restatement with the author's intended meaning;
3. the editor diagnoses the gap;
4. the text is revised at the smallest useful unit;
5. reader agents restate it again.

The goal is not simply to make the text sound better. The goal is to make the text easier to understand, easier to revise, and less likely to be misunderstood.

这个 skill 最核心的部件不是“一次性写出一段漂亮文字”，而是**修改 Loop**。

这个 Loop 的基本过程是：

1. 让不同读者 agent 复述自己理解到的内容；
2. 把读者复述和作者原意进行比较；
3. 诊断偏差来自结构、判断、例子、句子还是语气；
4. 修改最小有效单位；
5. 再让读者 agent 复述一次。

它的目标不是把文字“润色得更好听”，而是让文本更清楚、更可修改，也更不容易被误解。

## Install / 安装

Clone this repository into your Codex skills directory:

把这个仓库克隆到 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/codeAlpha1024/writing-loop-editor.git ~/.codex/skills/writing-loop-editor
```

Restart Codex or start a new chat so the skill metadata is reloaded.

然后重启 Codex，或开启一个新对话，让 skill 元数据重新加载。

## Update / 更新

To update an existing local install:

如果你已经安装过，后续更新可以运行：

```bash
cd ~/.codex/skills/writing-loop-editor
git pull
```

If you are maintaining this repository from the local source folder:

如果你是在本机维护这个仓库，可以这样提交更新：

```bash
cd "/Users/wastonalex/Documents/写作skill精炼"
python3 /Users/wastonalex/.codex/skills/.system/skill-creator/scripts/quick_validate.py .
git add .
git commit -m "Update writing loop skill"
git push
```

If you edited the installed local skill first, sync it back before committing:

如果你先修改的是本地已安装的 skill，提交前先同步回仓库：

```bash
cp ~/.codex/skills/writing_loop_editor/SKILL.md ./SKILL.md
```

## Use / 使用

Example prompts:

示例提示词：

```text
Use $writing-loop-editor to rewrite this passage with reader-agent diagnosis first.
调用三层写作Loop，检查这节是否清楚。
Use $writing-loop-editor to expand this outline into textbook prose.
用读者agent复述一下这段文字，看理解有没有偏差。
把这段扩写成教材正文。
```

The skill is designed to trigger on English writing and revision requests such as `long-form article`, `rewrite this passage`, `expand this section`, `reader-agent diagnosis`, `clarity check`, and `textbook chapter`.

它也会响应中文触发词，例如 `三层写作Loop`、`写作Loop`、`自升级编辑`、`读者agent`、`复述检查`、`检查是否清楚`、`反复优化`、`改文章`、`把这段改成`、`扩写`、`写入正文`。

## Repository Layout / 仓库结构

```text
SKILL.md              Codex skill instructions and trigger metadata
agents/openai.yaml    UI metadata for skill display
三层写作Loop/          Source design notes and writing-style references
```

```text
SKILL.md              Codex 实际读取的 skill 指令和触发元数据
agents/openai.yaml    skill 在界面中的展示信息
三层写作Loop/          原始设计文档和文风参考
```

## Maintenance Notes / 维护说明

The most important trigger surface is the `description` field in `SKILL.md` frontmatter. If the skill fires too broadly or too narrowly, edit that description first.

最重要的触发表面是 `SKILL.md` 顶部 frontmatter 里的 `description` 字段。如果 skill 触发得太宽或太窄，优先修改这里。

After changing the skill, validate it before pushing:

修改 skill 后，推送前先校验：

```bash
python3 /Users/wastonalex/.codex/skills/.system/skill-creator/scripts/quick_validate.py .
```
