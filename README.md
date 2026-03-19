# 日常总结 / Daily Summary

[中文](#中文) | [English](#english)

---

## 中文

通过问答式对话帮助用户总结一天的生活，养成每日复盘的习惯。

### 功能

- 🎯 **触发词**：今日总结、总结今天、今天总结、每日总结
- 💬 **问答式**：依次问四个问题，简洁不追问
- 📝 **持久记录**：内容追加写入 `memory/日常总结.md`，按日期分隔

### 四个问题

1. 今天做了什么？
2. 今天学了什么？
3. 今天做错了什么？
4. 明天需要做什么？

### 安装

```bash
npx clawhub@latest install daily-reflection
```

### 使用

说"今日总结"即可触发。

### 示例输出

```markdown
## 2026-03-19（周三）22:54

**今天做了：**
1. 下午去开会（项目交接）
2. 晚饭和朋友吃烤串

**今天学了：** 看了下 codex 的使用

**做错的：** 和朋友讨论时没有及时沟通感受

**明天要做：**
1. 看下项目代码
2. 看下需求情况

---
```

---

## English

A skill that helps you reflect on your day through a simple Q&A dialogue.

### Features

- 🎯 **Triggers**: "daily summary", "summarize today", "今日总结"
- 💬 **Q&A Style**: Asks four simple questions, no follow-ups
- 📝 **Persistent Log**: Appends to `memory/日常总结.md`, separated by date

### Four Questions

1. What did you do today?
2. What did you learn today?
3. What did you do wrong today?
4. What do you need to do tomorrow?

### Install

```bash
npx clawhub@latest install daily-reflection
```

### Usage

Say "daily summary" to trigger.

### Example Output

```markdown
## 2026-03-19（Wed）22:54

**Today I did:**
1. Meeting in the afternoon (project handover)
2. Dinner with friends

**Today I learned:** Explored codex usage

**What went wrong:** Didn't communicate feelings during discussion

**Tomorrow I will:**
1. Review project code
2. Check requirements

---
```

### License

MIT
