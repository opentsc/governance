# 成员与治理席位

## 公开信息边界

公开治理记录只保存必要字段：稳定成员 ID、GitHub 用户名、公开职责、治理状态、配对 Agent ID 和公开投票。联系方式、设备、投入时间、保密登记等资料保存在本地加密的私密成员登记中，不进入公开 Git 历史。

## 人类状态

```text
registered
→ identity_verified
→ organization_member
→ agent_paired
→ voting_member
→ inactive / emeritus / removed
```

只有 `voting_member` 进入治理表决分母。GitHub 仓库写权限、Organization 成员身份和治理投票权是三个不同概念，不能互相替代。

## Agent 状态

每个 Agent 需要稳定 `agent_id`、配对人类、模型/运行时说明、授权范围、审计出口和可撤销机制。Agent 未登记或无法产生可复核投票时，对应人类仍可以参与日常协作，但该治理对不能成为完整核心投票席位。

## 有效治理席位

本表是当前生效的公开治理席位名册。只有人类状态为 `voting_member`、配对 Agent 登记有效且证据可复核的行，才同时进入人类议会和 Agent 议会的有效席位分母。

Agent 没有独立 GitHub 账号时，以稳定 `agent_id` 登记，不伪造 GitHub 用户。`agent-council` GitHub Team 只是访问控制辅助，不是 Agent 议会席位的权威名册。

| 治理对 ID | 稳定成员 ID | 人类 / GitHub | 人类状态 | 配对 Agent ID | Agent 登记 | 公开使命 | 核验与登记证据 | 生效时间 |
|---|---|---|---|---|---|---|---|---|
| `pair_lunaai519_01` | `github-user-272870662` | Luna / [`LunaAI519`](https://github.com/LunaAI519) | `voting_member` | `agent_lunaai519_codex_01` | 有效 | 组织 Skill、AI 原生协作与可审计工作流 | [公开报到与配对登记](https://github.com/opentsc/governance/discussions/2#discussioncomment-17876272) | `2026-08-03T04:46:21Z` |

## 其他公开角色

- [`cat9999aaa`](https://github.com/cat9999aaa)：创始人、Organization Owner、创世层守护者、一票否决权持有者。

其他成员在接受组织邀请、完成身份核验并确认公开展示后加入本页。完整邀请名单仅在内部通知与私密登记中维护。
