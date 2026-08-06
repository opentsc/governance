# Godot AI Studio — 协作模式（2026-08-05 由项目负责人确立）

> 本文件是 godot-ai-studio 团队协作规则的唯一权威来源。产品仓库的
> `AGENTS.md` 与 `docs/community/task-board.md` 只保留工程协议与产品任务卡，
> 协作规则一律指向此处。

## 核心原则

- **核心代码由 cat9999aaa（主线负责人）一路前推**：交互 Surface、VRM、AI 制片组、
  SDK 等硬核模块直接写、直接验证、直接 PR，不做大等待、不做委员会式设计。
- **团队补配套**：其余成员与 Agent 按 [assignments.md](assignments.md) 的分工卡
  领取复现、证据、文档、评审、平台覆盖任务，为核心推进让路并兜底质量。
- **硬性合并纪律**：禁止直推 main、禁止 force-push、禁止本地 `refs/pr/*` 合并
  工具，一切改动走 GitHub PR + 绿 CI。背景：2026-08-04 一次直推覆盖了 6 个
  已合并 PR（含主线冲刺计划与视觉验收证据），当日已全部恢复。

## 进度真相来源

- 带日期的主线时间表：产品仓库 `docs/product/mainline-schedule.md`（每周一核对）。
- 波次验收标准：产品仓库 `docs/product/roadmap.md` 与
  `docs/product/acceptance/razzhood-mainline.md`。

## 关联组织项目

- **opentsc/agent-guard**：Agent 协作基础设施（fenced lease / IRC 生命周期
  消息），2026-08-06 从产品仓库迁出独立立项。原始设计实现：Luna；
  整合合并：jaycehuang。
