# BankGPT Skills

Reusable [Agent Skills](https://agentskills.io/) for [BankGPT](https://bankgpt.io/) workflows, bookkeeping, financial planning, spreadsheet analysis, and business operations. Each skill starts with a `SKILL.md` that describes when to use it, its inputs, and its workflow.

## Start with your business goal

Describe your business goal, the files or data you have, and the result you need. Start with one of these skills.

| Skill | When to use it | Example prompt | Topics |
| --- | --- | --- | --- |
| [bankgpt-skill-navigator](skills/bankgpt-skill-navigator/SKILL.md) | Find the right skill for your task. It explains why the skill fits and what inputs it needs. | Use $bankgpt-skill-navigator to recommend a skill for converting PDF bank statements into Excel and checking that the balances reconcile. | skill-discovery, task-routing, workflow-recommendations |
| [bankgpt-skill-composer](skills/bankgpt-skill-composer/SKILL.md) | Plan a task that needs multiple skills. It recommends which skills to use, in what order, and what each step passes to the next. | Use $bankgpt-skill-composer to plan a month-end close from PDF bank statements and a ledger export. Recommend the skills and show the handoffs. | workflow-orchestration, skill-composition, data-handoffs |

## Available Skills

### Financial Data and Bookkeeping

| Skill | What it does | Topics |
| --- | --- | --- |
| [bankgpt-workflow](skills/bankgpt-workflow/SKILL.md) | Generate invoices, scan receipts and PDFs, compare or merge tables, and summarize financial data in BankGPT. | financial-data, invoice-generation, document-scanning, table-comparison |
| [bookkeeping-close](skills/bookkeeping-close/SKILL.md) | Categorize transactions, reconcile statements against the ledger, and prepare a month-end close package. | bookkeeping, bank-reconciliation, month-end-close |
| [financial-parser](skills/financial-parser/SKILL.md) | Extract data from invoices, receipts, and statements, categorize expenses, and identify recurring charges. | document-extraction, expense-categorization, recurring-payments |
| [statement-extract-and-prove](skills/statement-extract-and-prove/SKILL.md) | Convert statement PDFs to CSV or Excel and verify transactions against balances and totals. | bank-statements, pdf-to-excel, balance-verification |

### Forecasting, Planning, and Pricing

| Skill | What it does | Topics |
| --- | --- | --- |
| [budget-optimizer](skills/budget-optimizer/SKILL.md) | Review spending and subscriptions and build a plan for savings, debt repayment, and emergency funds. | budgeting, expense-analysis, debt-repayment, emergency-funds |
| [cash-flow-forecaster](skills/cash-flow-forecaster/SKILL.md) | Build a rolling 13-week cash forecast from bank data, receivables, payables, payroll, and recurring commitments. | cash-flow-forecasting, accounts-receivable, accounts-payable |
| [financial-goal-planner](skills/financial-goal-planner/SKILL.md) | Set monthly savings targets and milestones for goals such as a down payment, education, or retirement. | financial-planning, savings-goals, retirement-planning |
| [tax-strategy-optimizer](skills/tax-strategy-optimizer/SKILL.md) | Compare U.S. tax planning scenarios involving pre-tax and Roth contributions, charitable giving, capital gains, and deductions. | us-tax-planning, roth-contributions, capital-gains, tax-deductions |
| [trade-quote-builder](skills/trade-quote-builder/SKILL.md) | Turn a field-service scope into a cost estimate and client quote with labor, materials, overhead, and margin. | field-services, cost-estimation, pricing, profit-margin |

### Spreadsheets, BI, and Reporting

| Skill | What it does | Topics |
| --- | --- | --- |
| [bi-measure-builder](skills/bi-measure-builder/SKILL.md) | Build and debug Power BI DAX, Tableau calculations, and Looker LookML with checkable expected results. | business-intelligence, power-bi, dax, tableau, lookml |
| [executive-dashboard-generator](skills/executive-dashboard-generator/SKILL.md) | Turn data into executive reports with key metrics, charts, and trend analysis. | executive-reporting, dashboards, kpi-tracking, data-visualization |
| [spreadsheet-model-auditor](skills/spreadsheet-model-auditor/SKILL.md) | Audit models for formula errors, inconsistent ranges, hardcoded values, and totals that do not reconcile. | spreadsheet-audit, formula-validation, financial-modeling |
| [spreadsheet-qa](skills/spreadsheet-qa/SKILL.md) | Answer questions about spreadsheet exports with reproducible calculations, filters, and supporting rows. | spreadsheet-analysis, data-quality, reproducible-analysis |

### Business Operations

| Skill | What it does | Topics |
| --- | --- | --- |
| [bankgpt-contract-renewal-radar](skills/bankgpt-contract-renewal-radar/SKILL.md) | Extract renewal dates, notice deadlines, and price increases into a renewal calendar. | contract-management, renewals, notice-deadlines |
| [bankgpt-data-room-builder](skills/bankgpt-data-room-builder/SKILL.md) | Organize a data room for fundraising, acquisition, or bank diligence and identify missing documents. | virtual-data-room, due-diligence, document-management |
| [bankgpt-deal-room](skills/bankgpt-deal-room/SKILL.md) | Review contracts, financials, and other deal documents for risks, terms, and negotiation points. | deal-analysis, due-diligence, contract-review |
| [bankgpt-expense-audit](skills/bankgpt-expense-audit/SKILL.md) | Match receipts to statement lines and flag anomalies and expense policy violations. | expense-audit, receipt-matching, policy-compliance |
| [bankgpt-folder-organizer](skills/bankgpt-folder-organizer/SKILL.md) | Classify, rename, deduplicate, and index files in a folder or shared drive. | file-organization, deduplication, document-indexing |
| [bankgpt-invoice-chaser](skills/bankgpt-invoice-chaser/SKILL.md) | Build a receivables aging report and draft payment follow-ups based on how overdue each invoice is. | accounts-receivable, invoice-collection, aging-report |
| [bankgpt-qbr-builder](skills/bankgpt-qbr-builder/SKILL.md) | Prepare a quarterly business review from client records, usage data, and support activity. | quarterly-business-review, customer-success, usage-analytics |
| [bankgpt-rfp-response](skills/bankgpt-rfp-response/SKILL.md) | Build an RFP compliance matrix, flag unmet requirements, and draft a response from existing materials. | rfp-response, proposal-writing, requirements-mapping |
| [bankgpt-sop-writer](skills/bankgpt-sop-writer/SKILL.md) | Turn notes or transcripts into a standard operating procedure with steps, roles, and exceptions. | standard-operating-procedures, process-documentation, workflow-design |
| [bankgpt-tax-prep-organizer](skills/bankgpt-tax-prep-organizer/SKILL.md) | Organize tax documents for an accountant and list missing forms and open questions. | tax-preparation, document-management, tax-forms |
| [bankgpt-vendor-comparison](skills/bankgpt-vendor-comparison/SKILL.md) | Compare vendor proposals by total cost of ownership, contract terms, and negotiation points. | procurement, vendor-evaluation, total-cost-of-ownership |

## Usage

Load the relevant skill directory in your agent, then provide the source files and describe the output you want. Check the linked `SKILL.md` for any scripts, connectors, or host features the workflow requires.

Examples for `bankgpt-workflow`:

| Host | Example |
| --- | --- |
| Codex | `Use $bankgpt-workflow to compare these spreadsheets and summarize the differences.` |
| Claude Code standalone skill | `/bankgpt-workflow Generate an invoice from the attached data.` |
| Claude Code plugin | `/bankgpt-workflow:bankgpt-workflow Merge these tables into one workbook.` |

BankGPT Workflow accepts pasted financial data, supported attachments such as PDFs, images, CSV, XLSX, TSV, and structured JSON, and local file paths when the agent has filesystem access. Convert audio or video to structured data before analysis. For comparisons, it reports mismatches, duplicates, and missing rows. For merges, it preserves source row order unless sorting is requested.
