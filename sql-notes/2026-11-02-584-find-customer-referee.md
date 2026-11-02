# 595. 大的国家（简单）
**日期**：2026-10-XX
**题意**：查出面积 ≥300万 或 人口 ≥2500万 的国家
**我的解法**：
SELECT name, population, area FROM World
WHERE area >= 3000000 OR population >= 25000000;
**错在哪 / 学到什么**：第一次忘了 OR 要用括号，和 AND 混用会出错
