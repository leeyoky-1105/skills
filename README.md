# Spec Skills — 14 个 Spec 文档写作引导 Skill

覆盖 Spec 文档全生命周期的引导式 AI Skill 集合，按六阶段流程逐步引导你完成从需求采集到追踪矩阵的完整文档体系。

## 六阶段流程

```
Proposal(03-04) → Spec(05-06-07) → Design(08-09-10-11) → Plan(12) → Test(13) → Trace(14)
  Why              What              How             When/Who     OK?      All linked?
```

## Skill 列表与触发方式

| 编号 | Skill 名称 | 触发方式（在对话中说） | 对应文档 |
|:---|:---|:---|:---|
| 01 | `spec-general` | "帮我建立 Spec 文档体系"、"初始化 Spec 编号"、"Spec 写作规则是什么" | 01-Spec写作总则与文档编号索引 |
| 02 | `spec-elicitation` | "帮我采集需求"、"记录需求来源"、"整理会议纪要中的需求" | 02-需求来源与采集记录 |
| 03 | `spec-proposal` | "帮我写立项提案"、"生成项目提案"、"定义项目范围" | 03-立项提案与范围说明 |
| 04 | `spec-prd` | "帮我写 PRD"、"生成产品需求说明"、"定义产品规则" | 04-产品需求说明 |
| 05 | `spec-user-story` | "帮我写用户故事"、"拆分 User Story"、"定义验收标准" | 05-用户故事与验收标准 |
| 06 | `spec-fsd` | "帮我写功能规格"、"定义界面行为"、"FSD 怎么写" | 06-功能规格说明 |
| 07 | `spec-nfr` | "定义非功能需求"、"写 NFR"、"定义性能指标" | 07-非功能需求与约束 |
| 08 | `spec-architecture` | "帮我写架构文档"、"定义系统架构"、"技术选型怎么写" | 08-系统架构与技术选型 |
| 09 | `spec-api-spec` | "帮我写 API 规格"、"定义接口契约"、"API 文档怎么写" | 09-API接口规格 |
| 10 | `spec-data-model` | "帮我写数据模型"、"定义数据表结构"、"Storage 方法怎么设计" | 10-数据模型与存储规格 |
| 11 | `spec-security` | "帮我写安全设计"、"定义安全规格"、"安全怎么做" | 11-安全设计规格 |
| 12 | `spec-plan` | "帮我写实施计划"、"定义里程碑"、"WBS 怎么拆" | 12-实施计划与里程碑 |
| 13 | `spec-test-strategy` | "帮我写测试策略"、"定义测试计划"、"质量门禁怎么设" | 13-测试策略与质量门禁 |
| 14 | `spec-traceability` | "帮我写追踪矩阵"、"建立需求追溯"、"检查覆盖率" | 14-需求追踪矩阵 |

## 推荐使用顺序

按六阶段顺序使用效果最佳，每一轮的输出作为下一轮的输入：

1. `spec-general` → 建立文档体系和编号规范
2. `spec-elicitation` → 采集需求来源
3. `spec-proposal` → 写立项提案（Why）
4. `spec-prd` → 写产品需求（What）
5. `spec-user-story` → 拆分用户故事
6. `spec-fsd` → 定义功能规格
7. `spec-nfr` → 定义非功能约束
8. `spec-architecture` → 定义系统架构
9. `spec-api-spec` → 定义 API 契约
10. `spec-data-model` → 定义数据模型
11. `spec-security` → 定义安全设计
12. `spec-plan` → 定义实施计划
13. `spec-test-strategy` → 定义测试策略
14. `spec-traceability` → 建立追踪矩阵

## 核心设计理念

每个 Skill 都遵循以下原则：

- **AI 负责引导提问和结构化整理**，人负责提供真实的业务信息
- **🛑 红线标记**：关键业务信息处标注红线，防止 AI 臆造
- **幻觉防御**：明确区分"AI 可以做"和"AI 绝不可以做"
- **协作关系**：每个 Skill 定义了与其他 Skill 的上下游关系
