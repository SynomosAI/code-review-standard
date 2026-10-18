# code-review-standard

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.md)
[![Agent Skill](https://img.shields.io/badge/Agent%20Skill-SKILL.md-blue.svg)](SKILL.md)
[![Code Review](https://img.shields.io/badge/code-review-checklist-brightgreen.svg)](SKILL.md)
[![Quality Gate](https://img.shields.io/badge/quality-gate-2ea44f.svg)](SKILL.md)

SynomosAI 四支柱体系：**身份（Identity）· 溯源（Traceability）· 治理（Governance）· 共生（Symbiosis）**——当 AI 进入商业，可信是唯一的硬通货。

> 本仓库属于 [SynomosAI](https://github.com/SynomosAI) 生态技能包的一员。生态全景见 [`synomosai-skills`](https://github.com/SynomosAI/synomosai-skills)，理论站位见 [`traceability-audit`](https://github.com/SynomosAI/traceability-audit)。

**关键词 / Keywords**：代码审查 · PR review · 质量门禁 · 检查清单 · Blocker / Suggestion / Nit · 工程规范 · code review checklist

## 🚀 快速开始 / Quick Start

本仓是一个 **Agent Skill 发布包**（遵循 SKILL.md 规范），不是可运行的 SDK。

```bash
# 1. 克隆本仓
git clone https://github.com/SynomosAI/code-review-standard.git
cd code-review-standard

# 2. 查看技能主文件（审查标准 / 检查清单 / 流程模板）
cat SKILL.md
```

```bash
# 3. 查看技能元信息
head -15 SKILL.md

# 4. 把技能目录放入你的 Agent 技能目录
#    cp -r . ~/.workbuddy/skills/code-review-standard/
```

## 仓库内容

代码审查标准

本技能提供一套完整的代码审查规范，覆盖三大铁律（教育优先 / 具体可操作 / 优先分级）、三级检查清单（🔴 Blockers / 🟡 Suggestions / 💭 Nits）、标准审查流程、Hotfix 紧急通道、自动化工具集成（ESLint / Prettier / Jest / SonarQube）、审查质量度量指标，以及 Blocker / Suggestion / Nit / 称赞四类评论模板。

## 元信息

- **技能名**：`code-review-standard`
- **版本**：1.0.0
- **署名**：SynomosAI
- **许可**：MIT（详见仓库 LICENSE）

## 使用方式

1. 克隆本仓库或将该技能目录放入你的 Agent 技能目录（如 `~/.workbuddy/skills/`）；
2. 在 Agent 中按 `SKILL.md` 的描述触发对应能力；
3. 需要审计/合规证据的场景，参考 `SKILL.md` 内模板产出工件。

## 审查流程概览

标准流程为：开发者自评 → 创建 PR → 审查者 24h 内响应 → 按检查清单审查 → 给出分级反馈 → 开发者修改 → 审查者确认 → Approve。紧急 Hotfix 走快速通道：资深工程师 30 分钟内审查，事后 24h 补全测试与文档。

```text
开发者完成开发 → 自评 → 创建 PR → 审查者 24h 响应
  → 按清单审查（Blocker / Suggestion / Nit）
  → 开发者修改并回复每条评论 → 审查者确认 → Approve
```

## 仓库结构 / Repository layout

```text
code-review-standard/
├── README.md              # 本文件
├── README.en.md           # 英文版说明
├── SKILL.md               # 技能主文件（审查标准 / 清单 / 模板 / 流程）
├── LICENSE.md             # MIT License
├── llms.txt               # 给 AI 的最小索引
├── llms-full.txt          # 给 AI 的完整文本
├── AGENTS.md              # 给 AI Agent 的工作指引
├── SECURITY.md            # 安全策略
└── .github/CODEOWNERS      # 代码所有者
```

## License / 许可

本项目以 **MIT** 许可发布，详见仓库根目录 [LICENSE.md](LICENSE.md)。版权：© 2026 注册老炮@MedXpert。

---

## 免责声明

本仓库内容为 SynomosAI 的**理论站位与工具化探索**，不代表任何已获认证、已商业化交付或已服务特定客户的声明；文中涉及的 ISO/IEC 42001、NIST AI RMF、GB/Z 185 等外部标准与条款信息为公开资料转述，正式引用前请**独立核实**。API、授权码与形象大使等为路线图（roadmap）事项，尚未上线。
