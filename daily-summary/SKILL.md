---
name: daily-summary
description: Daily life summary through Q&A dialogue. Triggers when user says "今日总结", "总结今天", "今天总结", "每日总结", "daily summary", "summarize today". Asks four questions (what you did, what you learned, what went wrong, what to do tomorrow) and appends entries to a single file. Use when user wants to reflect on their day.
---

# 日常总结 / Daily Summary

通过问答式对话帮助用户记录一天的生活。

## 工作流程

### 1. 确认日期时间

获取今天的日期和当前时间：
- 文件路径：`memory/日常总结.md`（固定一个文件）
- 如果文件已存在，追加新内容到文件末尾
- 如果文件不存在，创建新文件

### 2. 开启对话

用轻松自然的语气开始，例如：
> "好，我们来回顾一下今天。我问你答，想到什么说什么就行。"

### 3. 提问引导

依次问以下问题，简洁直接：

1. **今天做了什么？**
2. **今天学了什么？**
3. **今天做错了什么？**
4. **明天需要做什么？**

**原则：**
- 不追问细节
- 用户说"没有"就直接跳过进入下一个问题
- 保持简短，像随口一问

### 4. 写入文件

对话结束后，整理内容并写入文件：

```markdown
## YYYY-MM-DD（星期X）HH:MM

**今天做了：** [用户描述]

**今天学了：** [用户描述，无则写"无"]

**做错的：** [用户描述，无则写"无"]

**明天要做：** [用户描述，无则写"无"]

---
```

**写入规则：**
- 新总结追加在文件末尾
- 每条总结用日期时间作为标题
- 总结之间用 `---` 分隔

### 5. 结束对话

写入完成后，告诉用户文件路径：
> "记下来了，文件在 `memory/日常总结.md`"

## 注意事项

- 语气自然轻松，像朋友聊天
- 不要一次问太多问题，一次一个问题
- 用户不想回答的可以跳过
- 如果用户说"没了"、"就这些"，可以结束提问
- 文件操作前确保 `memory/` 目录存在
