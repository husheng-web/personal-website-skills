# 个人网站skill

一组面向作品集与个人网站的 Codex Skills。它们把反复出现、容易失真的工作拆成可复用流程：先保证内容可信，再保证页面、媒体、双语、动效和发布质量。

## 适用范围

适用于已有代码库、内容模型或设计规范的个人网站/作品集。每个 Skill 都要求先读取项目既有约定；它们不会替代项目事实、设计决策或发布授权。

## Skills

| Skill | 用来做什么 | 能解决什么问题 |
| --- | --- | --- |
| `portfolio-content-intake` | 盘点图片、PDF、链接和项目资料，形成可发布内容简报。 | 分离已证实事实、待确认说法和缺失信息，避免把素材或文件名误写成公开事实。 |
| `portfolio-case-production` | 在既有网站中新增或更新项目案例页。 | 让项目注册、叙事内容、组件和双语状态保持分层；材料不完整时诚实呈现部分案例。 |
| `portfolio-visual-qa` | 用设计参考图检验网页的桌面与移动端呈现。 | 找出层级、排版、间距、颜色、素材、响应式和交互中的可复现差异，并按优先级给出修复建议。 |
| `portfolio-bilingual-qa` | 审查中文与英文版本的页面和发布信息。 | 检查路由、切换、状态文案、metadata、sitemap 与文本换行，避免用未经批准的翻译填补事实空白。 |
| `portfolio-motion-qa` | 审查或实现网站动效。 | 保证动效使用已有 Token 和组件，并在 reduced-motion、键盘操作、性能和移动端上保持可用。 |
| `portfolio-media-asset-ops` | 准备、优化、替换和注册图片、长图与文档素材。 | 保留素材来源和原件，统一尺寸、alt 文本、数据引用与响应式表现，避免误删或错误替换。 |
| `portfolio-pages-release-check` | 在 GitHub Pages 静态发布前做完整检查。 | 核对构建、静态导出、站点 URL、sitemap、工作流和发布产物；它只检查，不会未经授权发布。 |
| `portfolio-project-preview-reader` | 为项目归档接入长图、文档页或阶段模块阅读器。 | 保持素材顺序、无障碍标签、对话框焦点/关闭行为和移动端无横向溢出。 |

## 使用方式

将本仓库中的 `skills/` 目录放入 Codex 的 Skill 目录，或按需复制单个 Skill 文件夹。每个文件夹都包含 `SKILL.md`：其中写明触发场景、工作边界、关键步骤与验证要求。

这些 Skill 默认可被自动匹配；也可以在任务中通过 `$skill-name` 显式调用，例如：

```text
使用 $portfolio-visual-qa 对照参考图检查 /zh/projects 页面。
```

## 设计原则

- **内容诚实**：未知事实保持待确认，未经批准的素材和英文文案不自动公开。
- **复用流程，而非复制页面**：Skill 固化的是判断与验证方式，不绑定某个具体项目、视觉风格或技术栈。
- **先检查后发布**：本仓库中的发布检查只提供证据与结论；推送、公开、部署等外部动作必须由当前任务明确授权。
- **尊重项目约定**：Skill 应扩展现有内容模型、组件、动效 Token 和部署方式，而不是引入平行体系。

## 仓库结构

```text
skills/
  portfolio-content-intake/
  portfolio-case-production/
  portfolio-visual-qa/
  portfolio-bilingual-qa/
  portfolio-motion-qa/
  portfolio-media-asset-ops/
  portfolio-pages-release-check/
  portfolio-project-preview-reader/
```

## 边界

本仓库不包含任何个人项目的原始资料、客户信息、私有链接、作品图片或未经确认的案例事实。它只公开可复用的工作方法。
