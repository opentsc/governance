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

## 当前公开角色

- [`cat9999aaa`](https://github.com/cat9999aaa)：创始人、Organization Owner、创世层守护者、一票否决权持有者。

其他成员在接受组织邀请、完成身份核验并确认公开展示后加入本页。完整邀请名单仅在内部通知与私密登记中维护。
