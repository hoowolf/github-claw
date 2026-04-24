# 项目级技能目录（.agents/skills）

本仓库所有项目级技能统一放在此目录下。

## 目录规范

- 技能根目录：`.agents/skills/`
- 每个技能独立目录：`.agents/skills/<skill-name>/`
- 每个技能目录至少包含：
  - `SKILL.md`：技能说明（用途、输入输出、边界、失败处理）
- 可选文件：
  - `install.sh`：技能依赖安装脚本（要求幂等）

## 发现与安装

- Copilot setup workflow 会扫描 `.agents/skills/*`
- 只有包含 `SKILL.md` 的目录会被识别为有效技能
- 若存在 `install.sh`，workflow 会自动执行安装

## 使用建议

- 主代理先匹配任务，再加载对应技能
- 无匹配技能时回退通用流程

## 官方技能来源

- 已安装 Anthropic 官方 skills：
  - 来源仓库：`https://github.com/anthropics/skills`
  - 同步范围：上游仓库 `skills/*` 下的技能目录（每个目录包含 `SKILL.md`）

## 更新方式

- 重新从官方仓库下载并覆盖 `.agents/skills/<skill-name>/`
- 保留本文件用于维护本仓库的技能目录规范
