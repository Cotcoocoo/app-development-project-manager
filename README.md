# App Development Project Manager

> A general-purpose Skill for managing the full lifecycle of application development: discovery, requirements, planning, design and engineering coordination, testing, release, and iteration.

[简体中文](#简体中文) · [English](#english)

## English

### What it does

`app-development-project-manager` helps an AI assistant manage application projects without confusing implementation progress with validated delivery. It supports Web, native mobile, mini programs, desktop apps, APIs/backends, AI products, and hybrid applications.

The Skill covers:

- Discovery, project facts, goals, scope, and success metrics
- Requirements, acceptance criteria, prioritization, and change control
- Milestones, tasks, dependencies, blockers, and ownership
- Design, technical, and quality gates
- Testing evidence, release readiness, rollback, and post-release checks
- Privacy, security, sensitive-data, third-party, and operational risks
- Status reports, decision logs, and iteration retrospectives

### Core behavior

- Separate **implemented**, **self-tested**, **tested**, **released**, and **user-validated** states.
- Treat dates, estimates, test results, and compliance claims as evidence-based facts; label unknowns as pending.
- Use milestones defined by verifiable outcomes, not calendar activity.
- Require acceptance criteria, dependencies, ownership, and a definition of done for executable tasks.
- Do not upload, publish, or externally share potentially sensitive project material without explicit authorization.

### Install

This repository follows the Agent Skills layout: `SKILL.md` is the required entry file.

1. Download or clone this repository.
2. Copy the `app-development-project-manager` folder into the skills directory supported by the target agent platform.
3. Restart or refresh the agent platform if it does not discover local skills automatically.

For WorkBuddy, this Skill can be kept in the user-level skills directory to make it available across projects, or in a project's `.workbuddy/skills/` directory to scope it to that project.

### Example prompts

- “Help me create a development plan for a cross-platform habit-tracking app.”
- “Turn this product requirement into executable tasks with acceptance criteria and dependencies.”
- “Give me a factual project status report; separate completed work from pending acceptance.”
- “Are we ready to release? Use a release-readiness checklist.”
- “Run a no-blame project retrospective and propose the next iteration.”

### Repository layout

```text
.
├── SKILL.md                         # The reusable Skill instructions
├── README.md                        # Overview and installation guidance
├── LICENSE                          # MIT License
├── CONTRIBUTING.md                  # Contribution workflow
├── CODE_OF_CONDUCT.md               # Community expectations
├── SECURITY.md                      # Vulnerability reporting guidance
├── SUPPORT.md                       # Usage and support channels
├── CHANGELOG.md                     # Release history
└── .github/
    ├── PULL_REQUEST_TEMPLATE.md
    └── ISSUE_TEMPLATE/
        ├── bug_report.yml
        ├── feature_request.yml
        └── config.yml
```

### License

Distributed under the [MIT License](LICENSE).

---

## 简体中文

### 这是什么

`app-development-project-manager` 是一套通用的应用开发全流程项目管理 Skill，帮助智能体协调从立项、需求、方案、设计与研发协作、测试验收、发布到迭代复盘的工作。

适用于 Web、iOS/Android 原生 App、小程序、桌面端、后端/API、AI 应用及混合项目。

### 核心能力

- 建立项目事实表：目标、用户场景、范围、约束、风险与成功指标
- 将需求转化为可验收的用户切片、任务、依赖与完成定义
- 管理优先级、变更、里程碑、阻塞项与跨角色协作
- 设置设计、技术与质量闸门，避免“代码完成”被误写为“验收完成”
- 管理测试证据、发布就绪清单、回滚与发布后验证
- 识别隐私、安全、敏感数据、第三方依赖、支付、合规和不可逆操作风险
- 输出简洁、可决策的项目状态报告与复盘结论

### 使用原则

- 严格区分：已开发、已自测、已测试通过、已发布、已被用户验证。
- 只把有证据的日期、工期、质量结论和合规结论写成事实；未知内容标为“待确认”或“未排期”。
- 使用可验证结果定义里程碑，而不是用“开会”“开始开发”等活动定义。
- 不在未获明确授权时上传、公开发布或对外发送可能包含敏感信息的项目资料。

### 安装

本仓库采用 Agent Skills 的标准结构，`SKILL.md` 是技能入口文件。

1. 下载或克隆本仓库；
2. 将 `app-development-project-manager` 文件夹复制到目标智能体平台支持的 skills 目录；
3. 如平台没有自动发现本地 Skill，重启或刷新平台。

在 WorkBuddy 中，可放入用户级 skills 目录以跨项目复用；若只想在一个项目中使用，可放入该项目的 `.workbuddy/skills/` 目录。

### 示例请求

- “帮我为一款跨平台习惯追踪 App 做开发计划。”
- “将这份需求拆成有验收标准和依赖关系的可执行任务。”
- “给我一份事实型项目状态报告，分开已完成和待验收内容。”
- “我们可以上线吗？按发布就绪清单评估。”
- “做一次不追责的项目复盘，并给出下一轮优先事项。”

### 许可证

本项目使用 [MIT License](LICENSE)。
