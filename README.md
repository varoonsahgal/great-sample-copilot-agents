# Amazing Copilot Studio Agents

> **50 production-ready declarative agents for Microsoft 365 Copilot.**
> Paste each instruction block into Copilot Studio → New agent → Instructions field.
> No coding required. Deploy in minutes.

> **50 production-ready agents across 13 domains.** See [AGENTS.md](AGENTS.md) for the complete library.

---

## What This Is

A curated library of instruction sets for [Microsoft 365 Copilot declarative agents](https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/overview-declarative-agent). Each agent is a paste-ready instruction block, ready to deploy without configuration files, coding, or Azure resources.

Every agent in this library:
- Requires a Microsoft 365 Copilot licence (the paid add-on — not included in standard M365 plans)
- Defaults to formal professional English (British spelling)
- Includes a banned vocabulary list to prevent AI-sounding language
- Includes a built-in quality self-check the agent runs before every response
- Stays within the 8,000-character Copilot Studio instruction limit

---

## How to Deploy Any Agent

1. Go to [m365.cloud.microsoft/chat/agent/new](https://m365.cloud.microsoft/chat/agent/new) — no separate tool needed, it's built into Microsoft 365 Copilot.
2. Enter the **Name** and **Description** from the agent file's frontmatter.
3. In the **Instructions** field, paste the full block from the `## Instructions` section of the relevant file.
4. Add knowledge sources (SharePoint sites) where noted.
5. Click **Create** — the agent is immediately available to `@mention` in Copilot Chat.

> You can also create agents via [Copilot Studio](https://copilotstudio.microsoft.com) for advanced configuration (additional knowledge sources, actions, authentication). For instruction-only agents in this library, the built-in Agent Builder is sufficient.

---

## Agent Directory

### Writing & Communication

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 01 | [**Enterprise Writer**](agents/writing-communication/enterprise-writer.md) | Draft and polish professional communications | All Staff | None | `@Enterprise Writer ...` |
| 02 | [**AI Text Humanizer**](agents/writing-communication/ai-text-humanizer.md) | Remove AI writing patterns from any text | All Staff | None | `@AI Text Humanizer ...` |
| 03 | [**Meeting Scribe**](agents/writing-communication/meeting-scribe.md) | Turn meeting notes into structured records | All Staff | None | `@Meeting Scribe ...` |

### Project Management

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 04 | [**Project Status Reporter**](agents/project-management/project-status-reporter.md) | Generate structured project status reports | PMs / Leadership | Optional: project SharePoint | `@Project Status Reporter ...` |
| 05 | [**Risk Register Manager**](agents/project-management/risk-register-manager.md) | Build and manage project risk registers | PMs | None | `@Risk Register Manager ...` |
| 06 | [**Document Reviewer**](agents/project-management/document-reviewer.md) | Review documents for quality and completeness | All Staff | None | `@Document Reviewer ...` |
| 07 | [**Lessons Learned Manager**](agents/project-management/lessons-learned-manager.md) | Convert retrospectives into structured LL entries | PMs / Leadership | Optional: LL SharePoint | `@Lessons Learned Manager ...` |
| 08 | [**Presentation Builder**](agents/project-management/presentation-builder.md) | Build structured slide outlines for any audience | Leadership / PMs | None | `@Presentation Builder ...` |
| 09 | [**Project Charter Writer**](agents/project-management/project-charter-writer.md) | Build a structured project charter from a brief | PMs / PMO | None | `@Project Charter Writer ...` |
| 10 | [**RAID Log Manager**](agents/project-management/raid-log-manager.md) | Generate and update RAID logs from meeting notes or project updates | PMs / PMO | None | `@RAID Log Manager ...` |

### HR & People

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 11 | [**Employee Onboarding Guide**](agents/hr-people/employee-onboarding-guide.md) | Answer new joiner questions | New Joiners / HR | Required: HR SharePoint | `@Onboarding Guide ...` |
| 12 | [**Job Description Writer**](agents/hr-people/job-description-writer.md) | Write clear, inclusive job descriptions | HR / Hiring Managers | None | `@Job Description Writer ...` |
| 13 | [**Performance Coach**](agents/hr-people/performance-coach.md) | Write SMART goals and structured performance feedback | All Staff / Managers | Optional: competency framework | `@Performance Coach ...` |
| 14 | [**Interview Question Builder**](agents/hr-people/interview-question-builder.md) | Generate structured, competency-based interview questions | HR / Hiring Managers | None | `@Interview Question Builder ...` |
| 15 | [**Exit Interview Analyser**](agents/hr-people/exit-interview-analyser.md) | Convert exit interview notes into a structured themes report | HR / People Analytics | None | `@Exit Interview Analyser ...` |

### Productivity

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 16 | [**Copilot Prompt Coach**](agents/productivity/copilot-prompt-coach.md) | Write and improve Copilot prompts | All Staff | None | `@Prompt Coach ...` |

### Finance

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 17 | [**Financial Report Writer**](agents/finance/financial-report-writer.md) | Draft management accounts commentary and board pack sections | Finance / Leadership | None | `@Financial Report Writer ...` |
| 18 | [**Budget Variance Analyst**](agents/finance/budget-variance-analyst.md) | Explain budget vs actual variances for management reporting | Finance / Controllers | None | `@Budget Variance Analyst ...` |
| 19 | [**Budget Justification Writer**](agents/finance/budget-justification-writer.md) | Convert a cost item list into a formal budget justification | Finance / PMs / Department Heads | None | `@Budget Justification Writer ...` |
| 20 | [**Board Paper Writer**](agents/finance/board-paper-writer.md) | Structure board-level papers with honest risk disclosure | CFO / CEO / Board Secretary | None | `@Board Paper Writer ...` |
| 21 | [**KPI Commentary Writer**](agents/finance/kpi-commentary-writer.md) | Take KPI results and write management commentary | Finance / FP&A / Business Partners | None | `@KPI Commentary Writer ...` |

### IT & Operations

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 22 | [**Incident Report Writer**](agents/it-ops/incident-report-writer.md) | Write IT incident post-mortems and reports | IT / Ops | None | `@Incident Report Writer ...` |
| 23 | [**Change Request Writer**](agents/it-ops/change-request-writer.md) | Write IT change management requests and CAB submissions | IT / Change Managers | None | `@Change Request Writer ...` |
| 24 | [**IT Request Scoper**](agents/it-ops/it-request-scoper.md) | Help non-technical staff write clear IT service requests | All Staff / Business Analysts | None | `@IT Request Scoper ...` |
| 25 | [**Runbook Writer**](agents/it-ops/runbook-writer.md) | Convert bullet-point procedures into structured runbooks | IT Ops / DevOps / Platform Engineers | None | `@Runbook Writer ...` |
| 26 | [**Security Risk Communicator**](agents/it-ops/security-risk-communicator.md) | Translate technical security findings into plain-language risk summaries | CISOs / Security Teams / Risk Committees | None | `@Security Risk Communicator ...` |

### Customer Success

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 27 | [**Escalation Handler**](agents/customer-success/escalation-handler.md) | Manage customer escalations with structured internal and external comms | CS / Account Managers | None | `@Escalation Handler ...` |
| 28 | [**Customer Response Writer**](agents/customer-success/customer-response-writer.md) | Write professional responses to customer queries and complaints | CS / Support | None | `@Customer Response Writer ...` |

### Sales & Business Development

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 29 | [**RFP Response Writer**](agents/sales/rfp-response-writer.md) | Write RFP responses and business proposals | Sales / BD | None | `@RFP Response Writer ...` |
| 30 | [**Sales Email Writer**](agents/sales/sales-email-writer.md) | Write outbound prospecting and follow-up emails | Sales / AEs | None | `@Sales Email Writer ...` |
| 31 | [**Account Plan Writer**](agents/sales/account-plan-writer.md) | Build structured account plans with stakeholder maps and relationship gaps | Account Managers / BD | None | `@Account Plan Writer ...` |
| 32 | [**Competitive Intelligence Brief**](agents/sales/competitive-intelligence-brief.md) | Produce competitor briefs and battle cards with confidence labelling | Sales / Marketing / Strategy | None | `@Competitive Intel ...` |
| 33 | [**Customer Case Study Writer**](agents/sales/customer-case-study-writer.md) | Write customer success stories in full, one-pager, and social formats | Marketing / Sales / CS | None | `@Case Study Writer ...` |

### Strategy & Executive

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 34 | [**Strategic Plan Structurer**](agents/strategy-executive/strategic-plan-structurer.md) | Structure multi-year strategic plans from executive input | C-Suite / Strategy Teams | None | `@Strategic Plan ...` |
| 35 | [**OKR Writer**](agents/strategy-executive/okr-writer.md) | Write, review, and cascade OKRs across teams | Leadership / Managers / Strategy | None | `@OKR Writer ...` |
| 36 | [**Executive Decision Brief**](agents/strategy-executive/executive-decision-brief.md) | Convert complex decisions into a one-page structured brief | C-Suite / Senior Leaders | None | `@Decision Brief ...` |

### Learning & Development

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 37 | [**Training Needs Analyser**](agents/learning-development/training-needs-analyser.md) | Convert performance gaps and survey data into structured TNA reports | L&D / HR / OD | None | `@Training Needs Analyser ...` |
| 38 | [**Course Outline Builder**](agents/learning-development/course-outline-builder.md) | Build structured course outlines with module sequencing and activity design | L&D / Instructional Designers | None | `@Course Outline Builder ...` |
| 39 | [**Assessment Question Writer**](agents/learning-development/assessment-question-writer.md) | Write scenario, MCQ, and short answer questions with marking criteria | L&D / Assessment Designers | None | `@Assessment Question Writer ...` |

### ESG & Sustainability

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 40 | [**ESG Report Section Writer**](agents/esg/esg-report-section-writer.md) | Draft ESG report sections aligned to GRI, TCFD, ESRS, or SASB | Sustainability Teams / CFOs | None | `@ESG Report Writer ...` |
| 41 | [**Carbon Footprint Narrative Writer**](agents/esg/carbon-footprint-narrative-writer.md) | Convert Scope 1, 2, and 3 emissions data into carbon narrative | Sustainability Teams / IR | None | `@Carbon Narrative ...` |

### Commercial & Legal

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 42 | [**Tender Response Writer**](agents/commercial-legal/tender-response-writer.md) | Structure technical and commercial responses to ITBs and RFPs | BD / Commercial / Proposal Managers | None | `@Tender Response Writer ...` |
| 43 | [**NDA & Agreement Summariser**](agents/commercial-legal/nda-agreement-summariser.md) | Summarise key clauses from NDAs and service contracts | Business Managers / Commercial / Procurement | None | `@NDA Summariser ...` |
| 44 | [**Compliance Checklist Builder**](agents/commercial-legal/compliance-checklist-builder.md) | Convert a regulation or policy into a structured compliance checklist | Compliance / Legal / Risk / Audit | None | `@Compliance Checklist ...` |
| 45 | [**Contract Language Simplifier**](agents/commercial-legal/contract-language-simplifier.md) | Rewrite dense contractual clauses into plain language | All Staff / Business Managers | None | `@Contract Simplifier ...` |
| 46 | [**Policy Summariser**](agents/commercial-legal/policy-summariser.md) | Convert long policy documents into what you must do, what is prohibited | HR / Compliance / All Staff | None | `@Policy Summariser ...` |

### Advanced / MCP-Enabled

> These agents require platform connections via Microsoft Graph API. Deploy after all instruction-only agents are stable.

| # | Agent | Description | Audience | Knowledge | Invoke |
|---|-------|-------------|----------|-----------|--------|
| 47 | [**SharePoint Knowledge Agent**](agents/advanced/sharepoint-knowledge-agent.md) | Answer questions grounded in a connected SharePoint site with source citations | All Staff | Required: SharePoint via Graph API | `@SharePoint Knowledge ...` |
| 48 | [**Email Triage Assistant**](agents/advanced/email-triage-assistant.md) | Classify, summarise, and draft responses to unread emails — never sends without confirmation | Senior Leaders / EAs / Chiefs of Staff | Required: Outlook via Graph API | `@Email Triage ...` |
| 49 | [**Meeting Intelligence Agent**](agents/advanced/meeting-intelligence-agent.md) | Produce structured records from Teams meeting transcripts | PMs / Team Leads / All Staff | Required: Teams transcripts via Graph API | `@Meeting Intelligence ...` |
| 50 | [**Cross-Agent Orchestrator**](agents/advanced/cross-agent-orchestrator.md) | Route user requests to the correct specialist agent — single entry point for the library | All Staff | All agents deployed | `@Copilot Assistant ...` |


---

## Notes

- All agents default to formal professional English with British spelling.
- Agents marked **Required knowledge source** will not answer outside that source. Connect the SharePoint site before publishing.
- The AI-assistance disclaimer present in several agents (meeting records, status reports) must be reviewed by the document owner before official distribution.
- Agent instructions are sized to stay within the 8,000-character Copilot Studio instruction limit.

---

## Full Library

The library contains 50 agents across 13 domains. See [AGENTS.md](AGENTS.md) for the complete index with links to every agent.

---




## Quick Links

- **[Agent Library](AGENTS.md)** — complete index of all 50 agents with links

---