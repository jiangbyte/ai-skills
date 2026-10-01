# AI Skills

![Cursor](https://img.shields.io/badge/Cursor-Rules%20%26%20Skills-000000?logo=cursor&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-Reserved-D97706)
![Codex](https://img.shields.io/badge/Codex-Reserved-10A37F)

**AI Skills** 是个人 AI Agent 的 skills / rules 配置仓库：按工具分目录存放，路径与本机配置同构（例如 Cursor 对应 `.cursor/`），方便在多个项目间复用与同步。

> 仓库：[jiangbyte/ai-skills](https://github.com/jiangbyte/ai-skills)

## 目录

- [工程结构](#工程结构)
- [Cursor Rules](#cursor-rules)
- [使用](#使用)

## 工程结构

```
ai-skills/
├── .cursor/           # Cursor
│   ├── rules/         # *.mdc
│   └── skills/        # 待整理（*/SKILL.md）
├── .claude/           # Claude Code（预留）
└── .codex/            # Codex（预留）
```

| 目录 | 工具 | 说明 |
| --- | --- | --- |
| `.cursor/rules` | Cursor | 项目级 Rules（`.mdc`） |
| `.cursor/skills` | Cursor | Agent Skills（待整理） |
| `.claude/` | Claude Code | skills / rules 预留 |
| `.codex/` | Codex | skills 预留 |

## Cursor Rules

| 文件 | 用途 |
| --- | --- |
| `api-interface.mdc` | API / 接口约定 |
| `chinese-comments.mdc` | 中文注释 |
| `code-change-discipline.mdc` | 改动纪律 |
| `database-operations.mdc` | 数据库操作 |
| `defensive-coding.mdc` | 防御性编码 |
| `error-logging.mdc` | 错误与日志 |
| `frontend-typescript.mdc` | 前端 TypeScript |
| `write-safety.mdc` | 写入安全 |

Rules 初始来自 [`jiangbyte/cursor/rules`](https://github.com/jiangbyte/jiangbyte/tree/main/cursor/rules)。

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
