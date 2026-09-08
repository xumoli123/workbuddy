# workbuddy — AI 概念学习资料库

本仓库汇集使用 **concept-learning-generator** Skill 生成的 AI 技术概念学习资料，以及该 Skill 本身。

## 📁 目录结构

```
workbuddy/
├── learning-materials/          # 概念学习资料（HTML，浏览器直接打开）
│   ├── agent.html               # Agent（智能体）
│   ├── llm-context.html         # 大模型的上下文（Context）
│   ├── skill.html               # Skill（技能）
│   └── concept-relationship.html # 三概念关系图（建议最后看）
├── .workbuddy/
│   └── skills/
│       └── concept-learning-generator/
│           └── SKILL.md         # 项目级 Skill 定义（严格按作业要求路径存放）
├── README.md
└── .gitignore
```

## 📖 学习资料说明

每份资料遵循统一的六模块结构，方便跨概念横向对比：

1. **个人通俗解释** — 生活化类比 + 严格定义
2. **核心机制** — 概念如何工作，解决了什么前置问题
3. **真实应用场景** — 真实产品/工程实践案例
4. **易混淆边界** — 相邻概念对比 + 记忆口诀
5. **权威参考链接** — arXiv 论文与官方来源，全部经实测可访问
6. **自测思考题** — 附可展开的参考答案要点

建议阅读顺序：`agent.html` → `llm-context.html` → `skill.html` → `concept-relationship.html`（把三者放进同一张图理解）。

## 🛠 生成新概念的学习资料

使用 `.workbuddy/skills/concept-learning-generator/SKILL.md` 中定义的流程：

- 输入：概念名称（如 RAG、KV Cache、Mixture of Experts），可选深度（入门/进阶/专家）
- 输出：六模块结构的 HTML 学习资料，保存至 `learning-materials/` 目录

## 📄 许可与说明

- 学习资料内容为个人学习笔记，参考链接版权归原作者/机构所有
- 全文简体中文，术语首次出现标注英文原文


## 人工核查与修改说明
1. 核对了三份学习资料中的外部参考链接，移除失效链接，替换为官方、权威技术文档来源。
2. 对Agent、大模型上下文、Skill的概念解释部分进行人工改写，使用个人通俗理解重新表述，去除AI生成的冗余套话。
3. 校验概念之间的逻辑关系，修正了AI生成内容中部分边界模糊的描述。
4. 修复三份学习资料中失效的外部参考链接，替换为主题匹配、可正常访问的权威技术文档来源。
5. 新增 `learning-materials/concept-relationship.html`，用关系图、区别对比表与速查表梳理 Agent、大模型上下文、Skill 三个概念之间的相互关系，并附权威参考来源链接。
6. 完善 `skills/concept-learning-generator/SKILL.md`：补充头部 YAML 元数据（name/description），确认其可接收任意 AI 概念作为输入的通用可复用项目级 Skill，并保留输出完整 HTML 学习文档结构的格式要求。
7. 按作业严格要求调整：将 SKILL.md 移动至 `.workbuddy/skills/concept-learning-generator/` 目录，符合 WorkBuddy 项目级 Skill 的标准存放路径。