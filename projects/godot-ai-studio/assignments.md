# Godot AI Studio — 当前任务分工（SUP 卡）

> 认领规则：每人/每个 Agent 只领自己名下的卡；完成后以 PR + 证据交付。
> 卡片状态变更由主线负责人每周一核对。

## SUP-01 — 第二台机器验收复跑（ozrwayne）
- 跟踪：godot-ai-studio #25
- 同一 main SHA、授权 PPTX，按 docs/product/acceptance/ppt-host-render.md 全流程，
  G1–G6 全 PASS 并产出 result.json/MP4/Manifest/截图/环境证据。

## SUP-02 — GDScript .uid 缺失修复（ozrwayne）
- 跟踪：godot-ai-studio #12
- 三个 GDScript 文件补 .uid；fresh clone + import 后 git status 干净。

## SUP-03 — Windows 复现（xiaoxihahaha）
- 跟踪：godot-ai-studio #66
- G1–G6 逐门 PASS/BLOCKED 结论 + 日志，阻塞项单独开 issue。

## SUP-04 — 视觉验收基线刷新（LunaAI519）
- 跟踪：godot-ai-studio #67
- 当前 main 重新采集 W2-06 基线，逐镜头标注回归。

## SUP-05 — 拆分 repository agent PR（GaryLauLGY）
- 跟踪：godot-ai-studio PR #63
- 拆为 ≤500 行可评审小 PR（models/store/workspace/CLI/tests），逐个绿 CI。

## SUP-06 — 评审与复现周常（miles-mzy、davinci-seven）
- 跟踪：godot-ai-studio #68 / #69
- 每周一项：复现一个具名验收检查，或评审一个开放 PR，带证据评论。

## SUP-07 — 流程归位（JayceHuang）
- 跟踪：godot-ai-studio #70
- 全部工作走 PR；agent-guard 已迁往 opentsc/agent-guard，后续在该仓库继续。
