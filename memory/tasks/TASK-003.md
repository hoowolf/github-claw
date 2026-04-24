# TASK-003 — 安装 Anthropic 官方 Skills

## 状态：✅ 完成

## 描述

将 Anthropic 官方 skills 仓库（`https://github.com/anthropics/skills`）中的官方技能安装到本仓库的项目级技能目录 `.agents/skills/`。

## 产出

- 安装并同步了以下官方技能目录：
  - `algorithmic-art`
  - `brand-guidelines`
  - `canvas-design`
  - `claude-api`
  - `doc-coauthoring`
  - `docx`
  - `frontend-design`
  - `internal-comms`
  - `mcp-builder`
  - `pdf`
  - `pptx`
  - `skill-creator`
  - `slack-gif-creator`
  - `theme-factory`
  - `web-artifacts-builder`
  - `webapp-testing`
  - `xlsx`
- 更新 `.agents/skills/README.md`，补充官方来源与更新方式

## 关键决策

- 采用“直接同步上游 `skills/*` 目录到本仓库 `.agents/skills/`”方式安装
- 保持现有技能发现机制不变（仍以 `SKILL.md` 作为有效技能识别标志）

## 完成于

2026-04-24
