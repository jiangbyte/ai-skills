# ai-skills

个人 AI Agent 的 **skills / rules** 仓库，按工具目录区分（与本机配置路径同构）。

| 目录 | 对应工具 | 说明 |
|------|----------|------|
| `.cursor/` | Cursor | `rules/*.mdc`、`skills/*/SKILL.md` |
| `.claude/` | Claude Code | skills / rules（预留） |
| `.codex/` | Codex | skills（预留） |

## Cursor

```
.cursor/
  rules/          # 从 jiangbyte/cursor/rules 迁入
  skills/
    ddd/          # DDD skill
    academic-blog-writing/
```

同步到某项目：

```bash
# rules
cp -a .cursor/rules/. /path/to/project/.cursor/rules/

# 或整棵挂接
ln -s "$(pwd)/.cursor" /path/to/project/.cursor
```

## 来源

- Rules：`jiangbyte/cursor/rules`
- Skills：从个人项目 `.cursor/skills` 汇总（`jiangbyte/cursor` 原先只有 rules）
