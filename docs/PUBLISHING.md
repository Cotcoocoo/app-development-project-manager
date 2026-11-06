# GitHub 发布清单

本目录已按 GitHub 公开仓库的常用社区健康文件结构整理完成。发布前按以下步骤操作。

## 1. 发布前人工确认

- 确认仓库名称建议为 `app-development-project-manager`。
- 确认愿意以 [MIT License](../LICENSE) 公开发布；如需限制商用、要求署名或采用其他许可证，先替换 `LICENSE` 并同步修改 README。
- 逐项检查 `SKILL.md`、`README.md`、`CHANGELOG.md`，确认没有客户名称、个人信息、内部策略、私有路径、账号、密钥或未公开产品信息。
- 确认初始版本号为 `1.0.0`；若希望采用其他版本号，在 `CHANGELOG.md` 中调整。

## 2. 创建 GitHub 仓库

1. 在 GitHub 新建仓库，名称使用 `app-development-project-manager`。
2. 选择公开或私有可见性；若希望他人复用和贡献，选择 Public。
3. 不在 GitHub 网页端额外初始化 README、LICENSE 或 `.gitignore`，因为本地目录已包含这些文件。
4. 创建完成后，将本地仓库关联到新仓库的远程地址。

## 3. 首次推送前检查

在仓库根目录运行：

```bash
git status
git diff --check
git add .
git diff --cached --check
```

确认暂存内容只包括：

- `SKILL.md`
- `README.md`
- `LICENSE`
- 社区健康文件和 GitHub 模板
- `.gitignore` 与 `.gitattributes`

不应暂存：`.env`、密钥、压缩包、依赖目录、构建产物、本地 `.workbuddy` 数据、个人或项目私有资料。

## 4. 首次提交与推送

创建清晰的初始提交，例如：

```text
feat: add app development project manager skill
```

关联 GitHub 远程后推送 `main` 分支。推送完成后，在 GitHub 仓库主页检查 README 是否正常渲染、许可证是否被识别、Issue 表单和 Pull Request 模板是否可用。

## 5. GitHub 仓库设置建议

- 在 About 中填写一句简短描述，例如：
  `A general-purpose AI skill for managing the full lifecycle of app development.`
- 添加主题：`agent-skill`、`project-management`、`app-development`、`product-management`、`ai-agent`。
- 在 Security 设置中启用 **Private vulnerability reporting**；`SECURITY.md` 已要求使用该渠道。
- 在 Settings → General 中确认 Issues 已启用；如需接收外部讨论，可再启用 Discussions。
- 在 Settings → Branches 中为 `main` 配置适度保护：要求拉取请求审查（如有协作者）及合并前状态检查（后续增加 CI 时）。
- 在发布第一个稳定版本后创建 GitHub Release `v1.0.0`，并引用 `CHANGELOG.md` 的对应条目。

## 6. 后续维护

- 行为变化：更新 `SKILL.md`、README 和 CHANGELOG。
- 修复或安全相关更新：在变更记录中说明影响和升级建议；不要公开敏感漏洞的利用细节，直到修复可用。
- 接收贡献：使用 CONTRIBUTING、Issue 表单和 PR 模板；避免接纳任何私有项目规则、用户数据或未验证的合规声明。
