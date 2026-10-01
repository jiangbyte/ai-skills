# AI Skills

![Cursor](https://img.shields.io/badge/Cursor-Rules%20%26%20Skills-000000?logo=cursor&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-Reserved-D97706)
![Codex](https://img.shields.io/badge/Codex-Reserved-10A37F)

**AI Skills** 是个人 AI Agent 的 skills / rules 配置仓库：按工具分目录存放，路径与本机配置同构（例如 Cursor 对应 `.cursor/`），方便在多个项目间复用与同步。

> 仓库：[jiangbyte/ai-skills](https://github.com/jiangbyte/ai-skills)

## 目录

- [工程结构](#工程结构)
- [使用](#使用)

## 工程结构

```
ai-skills/
├── .cursor/           # Cursor
│   ├── rules/         # *.mdc
│   └── skills/        # */SKILL.md
├── .claude/           # Claude Code（预留）
└── .codex/            # Codex（预留）
```

| 目录 | 工具 | 说明 |
| --- | --- | --- |
| `.cursor/rules` | Cursor | 项目级 Rules（`.mdc`） |
| `.cursor/skills` | Cursor | Agent Skills |
| `.claude/` | Claude Code | skills / rules 预留 |
| `.codex/` | Codex | skills 预留 |

## 使用

复制 Rules 到目标项目：

```bash
mkdir -p /path/to/project/.cursor/rules
cp -a .cursor/rules/. /path/to/project/.cursor/rules/
```

或挂接整棵 Cursor 配置：

```bash
ln -s "$(pwd)/.cursor" /path/to/project/.cursor
```
