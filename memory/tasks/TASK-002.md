# TASK-002 — 优化技能发现与安装机制

## 状态：✅ 完成

## 描述

优化仓库工作流与 `AGENTS.md`，建立项目级技能在主代理中的稳定发现、安装和使用机制。

## 产出

- `.github/workflows/copilot-setup-steps.yml`：新增 Copilot setup workflow，自动发现 `.agents/skills/*` 并执行技能 `install.sh`
- `.agents/skills/README.md`：新增技能目录规范说明
- `AGENTS.md`：新增技能目录、发现、安装、使用机制约定

## 关键决策

- 技能根目录固定为 `.agents/skills/`
- 每个技能目录必须独立，且以 `SKILL.md` 作为有效技能识别标志
- 安装逻辑由 setup workflow 统一触发，技能目录内 `install.sh` 自治、幂等

## 完成于

2026-04-24
