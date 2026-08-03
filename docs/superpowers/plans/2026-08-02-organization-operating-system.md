# Open TSC 组织操作系统实施计划

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** 将 `opentsc` GitHub Organization 建成可直接运行、中文优先、可持续进化的人机共治组织框架。

**Architecture:** `governance` 保存公开治理契约和协作入口，`.github` 提供组织级社区文件，`organization-infrastructure` 私密保存组织期望状态与审计运行手册。GitHub Discussions、Wiki、Projects、Teams 和仓库级保护共同构成当前运行壳。

**Tech Stack:** GitHub Organization、Git、Markdown、YAML、GitHub Actions、GitHub CLI、GitHub REST/GraphQL API。

## Global Constraints

- 中文是权威版本，英文只作为翻译。
- 不把邮箱、电话、微信、设备或投入时间写入公开仓库。
- 核心变更需全体有效人类席位和 Agent 议会一致同意，且创始人未否决。
- 创始人 `cat9999aaa` 保留 Owner 权限和一票否决权。
- Agent 议会建立前，核心法典保持“启动期草案”。
- GitHub Free 环境采用仓库级分支保护，不依赖组织级 Ruleset。

---

### Task 1: 建立治理中心

**Files:**
- Create: `README.md`
- Create: `GENESIS.md`
- Create: `GOVERNANCE.md`
- Create: `AI-CONSTITUTION.md`
- Create: `JUDGMENT-CODEX.md`
- Create: `ROADMAP.md`
- Create: `MEMBERS.md`
- Create: `policies/*.md`
- Create: `rfcs/*.md`
- Create: `adrs/*.md`

**Interfaces:**
- Consumes: TSC 3.0/3.5 白皮书、创始人确认的人机配对与否决权规则。
- Produces: 可被成员、Agent、模板和自动化引用的治理契约。

- [ ] **Step 1: 创建中文权威治理文档和目录。**
- [ ] **Step 2: 创建 RFC、ADR、Issue、Discussion 和 PR 模板。**
- [ ] **Step 3: 添加治理完整性检查工作流。**
- [ ] **Step 4: 运行本地文件与链接检查。**
- [ ] **Step 5: 提交并推送 `main`。**

### Task 2: 建立组织主页和默认社区文件

**Files:**
- Create: `profile/README.md`
- Create: `CONTRIBUTING.md`
- Create: `CODE_OF_CONDUCT.md`
- Create: `SECURITY.md`
- Create: `SUPPORT.md`
- Create: `.github/ISSUE_TEMPLATE/*.yml`
- Create: `.github/PULL_REQUEST_TEMPLATE.md`

**Interfaces:**
- Consumes: `governance` 的正式入口和中文优先政策。
- Produces: 组织主页与所有未自定义仓库继承的社区健康文件。

- [ ] **Step 1: 创建组织导航主页。**
- [ ] **Step 2: 创建默认 Issue 与 PR 模板。**
- [ ] **Step 3: 创建贡献、安全、支持和行为准则。**
- [ ] **Step 4: 提交并推送 `main`。**

### Task 3: 建立 Organization as Code

**Files:**
- Create: `org/settings.yml`
- Create: `org/repositories.yml`
- Create: `org/teams.yml`
- Create: `org/labels.yml`
- Create: `docs/runbook.md`
- Create: `scripts/verify-manifests.sh`
- Create: `.github/workflows/audit.yml`

**Interfaces:**
- Consumes: 当前 GitHub Organization 状态。
- Produces: 可版本化、可审阅、可用于人工或 Agent 审计的期望状态。

- [ ] **Step 1: 写入组织、仓库、团队和标签期望状态。**
- [ ] **Step 2: 创建只读验证脚本和 CI。**
- [ ] **Step 3: 运行验证脚本。**
- [ ] **Step 4: 提交并推送 `main`。**

### Task 4: 启用协作表面

**Files:**
- Create: GitHub Discussion 欢迎帖。
- Create: GitHub Wiki `Home` 页面。
- Create: GitHub Project “Open TSC 组织演化”。
- Create: `human-council`、`agent-council`、`maintainers`、`contributors` Teams。

**Interfaces:**
- Consumes: 治理文档和已接受邀请的成员名单。
- Produces: 论坛、知识入口、路线图和动态权限容器。

- [ ] **Step 1: 启用治理仓库 Discussions 和 Wiki。**
- [ ] **Step 2: 创建论坛欢迎帖与成员报到帖。**
- [ ] **Step 3: 初始化 Wiki 首页。**
- [ ] **Step 4: 创建并填充组织 Project。**
- [ ] **Step 5: 创建团队并加入当前正式成员。**

### Task 5: 配置权限与保护

**Files:**
- Modify: GitHub Organization settings。
- Modify: 各仓库 settings、security、branch protection。

**Interfaces:**
- Consumes: `organization-infrastructure/org/*.yml`。
- Produces: 与期望状态一致的 GitHub 实际配置。

- [ ] **Step 1: 设置中文组织资料和最小默认权限。**
- [ ] **Step 2: 禁止普通成员任意创建仓库。**
- [ ] **Step 3: 配置仓库功能、安全扫描和合并策略。**
- [ ] **Step 4: 在初始提交完成后启用仓库级分支保护。**
- [ ] **Step 5: 用 REST/GraphQL API 复核配置。**

### Task 6: 完成审计与成员通知

**Files:**
- Create: 线程内微信群通知文案。

**Interfaces:**
- Consumes: 实际成员、邀请、仓库、团队、论坛、Wiki、Project 和保护状态。
- Produces: 可直接发送到微信群的中文通知。

- [ ] **Step 1: 逐项核验显式需求和实际外部状态。**
- [ ] **Step 2: 区分已加入与待接受邀请名单。**
- [ ] **Step 3: 生成包含入口、行动要求和邀请名单的微信群文案。**
