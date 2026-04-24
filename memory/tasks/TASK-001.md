# TASK-001 — 初始化个人 AI 工作空间

## 状态：✅ 完成

## 描述

将 `hoowolf/github-claw` 仓库初始化为适合 GitHub Copilot 长期使用的个人 AI 工作空间。

## 产出

- `AGENTS.md`：核心身份与规则文件
- `MEMORY.md`：长期记忆文件
- `memory/` 目录结构（daily / tasks / context）
- 更新后的 `README.md`

## 关键决策

- 以 `AGENTS.md` 为唯一核心规范，其他文件均为辅助
- 记忆分四层：长期（MEMORY.md）/ 主题（context/）/ 日常（daily/）/ 任务（tasks/）
- 保持轻量：不过度设计，不创建无用文件

## 完成于

2026-04-24
