# 595. 大的国家（简单）

**日期**：2026-10-15
**考点**：`SELECT` / `WHERE` / `OR` 与 `AND` 的优先级

## 题意

找出**面积 ≥ 3000000** 或 **人口 ≥ 25000000** 的国家，输出 `name`、`population`、`area`。

## 我的解法

```sql
SELECT name, population, area
FROM World
WHERE area >= 3000000 OR population >= 25000000;
```

## 我错在哪 / 学到什么

- `OR` 和 `AND` 混用时**必须加括号**，否则优先级会让结果出错（AND 先算）。
- 同一个条件用 `OR` 连接时不需要括号，但养成随手加括号的习惯更安全。
- 这是 LeetCode 数据库第 1 题，主要用来熟悉**在线写 SQL + 提交**的环境。
