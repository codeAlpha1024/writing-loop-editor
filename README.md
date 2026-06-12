# Writing Loop Editor

Writing Loop Editor is a Codex skill for long-form prose writing and revision. It is designed for article-style Chinese or English writing where structure, reader understanding, evidence boundaries, and iterative revision matter.

Use it for:

- textbook or manuscript chapters;
- research essays and explanatory prose;
- commentary, analysis, policy briefs, or academic-style drafts;
- rewriting drafts for clearer structure and style;
- reader-agent restatement, clarity checks, and repeated revision loops.

Do not use it for ordinary chat, simple factual answers, code-only tasks, or isolated one-line copy edits unless you explicitly want to apply the writing loop.

## Install

Clone this repository into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/codeAlpha1024/writing-loop-editor.git ~/.codex/skills/writing-loop-editor
```

Restart Codex or start a new chat so the skill metadata is reloaded.

## Update

To update an existing local install:

```bash
cd ~/.codex/skills/writing-loop-editor
git pull
```

If you are maintaining this repository from the local source folder:

```bash
cd "/Users/wastonalex/Documents/写作skill精炼"
python3 /Users/wastonalex/.codex/skills/.system/skill-creator/scripts/quick_validate.py .
git add .
git commit -m "Update writing loop skill"
git push
```

If you edited the installed local skill first, sync it back before committing:

```bash
cp ~/.codex/skills/writing_loop_editor/SKILL.md ./SKILL.md
```

## Use

Example prompts:

```text
Use $writing-loop-editor to rewrite this passage with reader-agent diagnosis first.
调用三层写作Loop，检查这节是否清楚。
用读者agent复述一下这段文字，看理解有没有偏差。
把这段扩写成教材正文。
```

The skill is also designed to trigger on phrases such as `三层写作Loop`, `写作Loop`, `自升级编辑`, `读者agent`, `复述检查`, `检查是否清楚`, `反复优化`, `改文章`, `把这段改成`, `扩写`, and `写入正文`.

## Repository Layout

```text
SKILL.md              Codex skill instructions and trigger metadata
agents/openai.yaml    UI metadata for skill display
三层写作Loop/          Source design notes and writing-style references
```

## Maintenance Notes

The most important trigger surface is the `description` field in `SKILL.md` frontmatter. If the skill fires too broadly or too narrowly, edit that description first.

After changing the skill, validate it before pushing:

```bash
python3 /Users/wastonalex/.codex/skills/.system/skill-creator/scripts/quick_validate.py .
```
