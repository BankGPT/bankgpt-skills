# BankGPT 技能

这套可复用的 [Agent Skills](https://agentskills.io/) 涵盖 [BankGPT](https://bankgpt.io/) 工作流、记账、财务规划、电子表格分析和业务运营。每项技能的 `SKILL.md` 说明适用场景、所需输入和操作流程。

## 从业务需求开始

先说明你的业务目标、已有文件或数据，以及希望得到的结果，再选择下面的一项技能。

| 技能 | 什么时候用 | 示例提示词 |
| --- | --- | --- |
| [bankgpt-skill-navigator](skills/bankgpt-skill-navigator/SKILL.md) | 想知道哪个技能适合当前任务时使用。它会推荐技能，说明推荐理由和所需输入。 | 使用 $bankgpt-skill-navigator 推荐合适的技能。我想把 PDF 银行对账单转换为 Excel，并核对余额是否一致。 |
| [bankgpt-skill-composer](skills/bankgpt-skill-composer/SKILL.md) | 任务需要多个技能协作时使用。它会推荐技能组合，说明执行顺序和每一步需要交接的内容。 | 使用 $bankgpt-skill-composer 规划月末结账。我有 PDF 银行对账单和总账导出文件，请推荐技能并说明执行顺序和数据如何交接。 |

## 可用技能

### 财务数据与记账

| 技能 | 用途 |
| --- | --- |
| [bankgpt-workflow](skills/bankgpt-workflow/SKILL.md) | 在 BankGPT 中生成发票、扫描收据和 PDF、比较或合并表格，以及汇总财务数据。 |
| [bookkeeping-close](skills/bookkeeping-close/SKILL.md) | 对交易进行分类，将对账单与总账核对，并准备月末结账资料。 |
| [financial-parser](skills/financial-parser/SKILL.md) | 从发票、收据和对账单中提取数据，对支出进行分类，并识别周期性扣款。 |
| [statement-extract-and-prove](skills/statement-extract-and-prove/SKILL.md) | 将 PDF 对账单转换为 CSV 或 Excel，并使用余额和合计金额验证交易明细。 |

### 预测、规划与定价

| 技能 | 用途 |
| --- | --- |
| [budget-optimizer](skills/budget-optimizer/SKILL.md) | 审查支出与订阅，制定储蓄、还债和应急资金计划。 |
| [cash-flow-forecaster](skills/cash-flow-forecaster/SKILL.md) | 根据银行数据、应收款、应付款、工资和经常性支出承诺，编制滚动 13 周现金流预测。 |
| [financial-goal-planner](skills/financial-goal-planner/SKILL.md) | 为首付、教育或退休等目标设定每月储蓄额度和阶段性目标。 |
| [tax-strategy-optimizer](skills/tax-strategy-optimizer/SKILL.md) | 比较涉及税前缴款、Roth 缴款、慈善捐赠、资本利得和扣除项目的美国税务规划方案。 |
| [trade-quote-builder](skills/trade-quote-builder/SKILL.md) | 根据现场服务的工作范围编制成本估算和客户报价，涵盖人工、材料、间接费用和利润率。 |

### 电子表格、BI 与报告

| 技能 | 用途 |
| --- | --- |
| [bi-measure-builder](skills/bi-measure-builder/SKILL.md) | 编写和调试 Power BI DAX、Tableau 计算及 Looker LookML，并提供可核验的预期结果。 |
| [executive-dashboard-generator](skills/executive-dashboard-generator/SKILL.md) | 将数据整理成管理层报告，提供关键指标、图表和趋势分析。 |
| [spreadsheet-model-auditor](skills/spreadsheet-model-auditor/SKILL.md) | 审查模型中的公式错误、范围不一致、硬编码数值和无法核对的合计。 |
| [spreadsheet-qa](skills/spreadsheet-qa/SKILL.md) | 通过可复现的计算、筛选条件和明细行，回答有关电子表格导出数据的问题。 |

### 业务运营

| 技能 | 用途 |
| --- | --- |
| [bankgpt-contract-renewal-radar](skills/bankgpt-contract-renewal-radar/SKILL.md) | 提取续约日期、通知截止日期和涨价信息，并汇总到续约日历。 |
| [bankgpt-data-room-builder](skills/bankgpt-data-room-builder/SKILL.md) | 为融资、收购或银行尽调整理资料室，并识别缺失文件。 |
| [bankgpt-deal-room](skills/bankgpt-deal-room/SKILL.md) | 审查合同、财务资料和其他交易文件，梳理风险、条款及谈判要点。 |
| [bankgpt-expense-audit](skills/bankgpt-expense-audit/SKILL.md) | 将收据与对账单明细匹配，并标记异常和违反费用政策的项目。 |
| [bankgpt-folder-organizer](skills/bankgpt-folder-organizer/SKILL.md) | 对文件夹或共享云盘中的文件进行分类、重命名、去重和编制索引。 |
| [bankgpt-invoice-chaser](skills/bankgpt-invoice-chaser/SKILL.md) | 编制应收账款账龄报告，并根据各发票的逾期时间起草催款消息。 |
| [bankgpt-qbr-builder](skills/bankgpt-qbr-builder/SKILL.md) | 根据客户记录、使用数据和支持服务记录，准备季度业务回顾。 |
| [bankgpt-rfp-response](skills/bankgpt-rfp-response/SKILL.md) | 编制 RFP 要求符合性矩阵，标记未满足的要求，并利用现有材料起草响应文件。 |
| [bankgpt-sop-writer](skills/bankgpt-sop-writer/SKILL.md) | 将笔记或转录稿整理成标准操作规程，明确步骤、角色和例外情况。 |
| [bankgpt-tax-prep-organizer](skills/bankgpt-tax-prep-organizer/SKILL.md) | 为会计师整理报税文件，并列出缺失表单和待确认事项。 |
| [bankgpt-vendor-comparison](skills/bankgpt-vendor-comparison/SKILL.md) | 按总拥有成本、合同条款和谈判要点比较供应商方案。 |

## 使用方法

在你的智能体中加载对应的技能目录，然后提供源文件并说明所需输出。请查看链接中的 `SKILL.md`，确认工作流所需的脚本、连接器或宿主平台功能。

以下示例使用 `bankgpt-workflow`。

| 使用环境 | 调用示例 |
| --- | --- |
| Codex | `使用 $bankgpt-workflow 比较这些电子表格并汇总差异。` |
| Claude Code 独立技能 | `/bankgpt-workflow 根据附件中的数据生成发票。` |
| Claude Code 插件 | `/bankgpt-workflow:bankgpt-workflow 将这些表格合并到一个工作簿中。` |

BankGPT Workflow 支持直接粘贴财务数据，也支持 PDF、图片、CSV、XLSX、TSV 和结构化 JSON 等附件。智能体具备文件系统访问权限时，也可以提供本地文件路径。音频或视频需先转换为结构化数据再分析。比较时会报告不一致、重复和缺失的行。合并时默认保留原始行顺序，可按要求排序。
