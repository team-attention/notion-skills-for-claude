# Notion Skills for Claude

Official Notion Skills created by Notion for Claude. These skills teach Claude how to complete real workflows in Notion.

> [Korean README](README.ko.md) | [Original Notion Page](NOTION.md)

## Source

This repository redistributes content from [Notion's official Skills for Claude page](https://www.notion.so/notiondevs/Notion-Skills-for-Claude-28da4445d27180c7af1df7d8615723d0) for **educational purposes**. It serves as a reference for understanding Claude Skills structure and implementation patterns.

## Overview

Notion Skills are step-by-step guides that help Claude complete entire workflows in Notion - structuring pages, updating databases, following patterns, and working through your actual processes.

## Available Skills

| Skill | Description |
|-------|-------------|
| [notion-meeting-intelligence](skills/notion-meeting-intelligence/) | Prepares meeting materials by gathering context from Notion, creating pre-reads and agendas |
| [notion-research-documentation](skills/notion-research-documentation/) | Synthesizes findings from multiple pages into structured research reports |
| [notion-knowledge-capture](skills/notion-knowledge-capture/) | Transforms conversations into structured documentation in Notion |
| [notion-spec-to-implementation](skills/notion-spec-to-implementation/) | Turns product/tech specs into concrete Notion tasks for implementation |

## Installation

### Claude.ai

1. Download the `.zip` file for the skill you want
2. Open **Settings** > **Capabilities** > **Skills**
3. Upload the `.zip` file
4. Click `...` > **Try in chat** to get started

### Claude Code

Copy the skill folder to your project or personal skills directory:

```bash
# Personal skills (available across all projects)
cp -r skills/notion-meeting-intelligence ~/.claude/skills/

# Project skills (shared with team)
cp -r skills/notion-meeting-intelligence .claude/skills/
```

## Skill Structure

Each skill follows the standard Claude Skills format:

```
skill-name/
├── SKILL.md           # Core instructions (YAML frontmatter + markdown)
├── evaluations/       # Test scenarios
├── examples/          # Usage examples
└── reference/         # Templates and guides
```

## Resources

- [What are Skills?](https://support.claude.com/en/articles/12512176-what-are-skills)
- [Using Skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude)
- [Agent Skills Documentation](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview)
- [Anthropic Skills Repository](https://github.com/anthropics/skills)

## License

These skills are provided by Notion. See individual skill folders for specific terms.
