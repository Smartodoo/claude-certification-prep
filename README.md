# Claude Certification Prep — study guide for CCAO-F, CCDV-F, CCAR-F and CCAR-P

A community study guide for Anthropic's four **Claude certifications**: what each exam tests, how
the domains are weighted, where the official documentation for each domain lives, and a preparation
plan that follows the weights instead of the table of contents. For each exam there is also a complete
video prep course on Udemy (see [the courses](#our-udemy-prep-courses) below).

> Independent and unofficial. Not affiliated with or endorsed by Anthropic. Exam names and codes
> belong to Anthropic. Figures marked *(exam guide v1.0, July 2026)* are taken from the official
> exam guides that Anthropic gives candidates at registration; always confirm against the guide for
> your exam date, because weights change between versions.

## The four certifications at a glance

| Code | Certification | Who it is for | Questions | Time | Official exam fee (USD, per attempt) |
|---|---|---|---|---|---|
| **CCAO-F** | Claude Certified Associate – Foundations | People who use Claude in their work without writing code: consultants, analysts, project leads, operations, legal, marketing | 60 | 120 min | $99 |
| **CCDV-F** | Claude Certified Developer – Foundations | Engineers building applications on the Claude API, tool use and agents | 53 | 120 min | $125 |
| **CCAR-F** | Claude Certified Architect – Foundations | Solution architects designing agent systems (orchestration, MCP, Claude Code) | 60 | 120 min | $125 |
| **CCAR-P** | Claude Certified Architect – Professional | Architects responsible for enterprise-scale deployments: integration, governance, evaluation, stakeholders | 63 | 120 min | $175 |

Common to all four *(exam guide v1.0, July 2026)*:

- The fee in the table is the **real exam fee** for Anthropic's certification exam, charged by
  Pearson VUE when you register: $99 for CCAO-F, $125 for CCDV-F and CCAR-F, $175 for CCAR-P. It
  has nothing to do with the price of any course or study material.

- Scenario-based multiple-choice items: judgment, not recall.
- Scaled score 100–1,000, **pass mark 720**.
- Proctored and identity-verified through Pearson VUE (online or test centre).
- Credential valid for **12 months**.
- Registration goes through the **Claude Partner Network** (membership is free): https://claude.com/partners
- Anthropic's announcement of the programme: https://claude.com/blog/four-role-based-claude-certifications

Which one first? If you write code, CCDV-F. If you design systems with agents, CCAR-F, then CCAR-P.
If you use Claude but do not build with the API, CCAO-F. The Architect Professional exam assumes
you have built with an LLM API in production; it is not a starting point.

---

## CCAO-F · Claude Certified Associate – Foundations

### Domains and weights *(exam guide v1.0, July 2026)*

| # | Domain | Weight |
|---|---|---|
| 1 | Prompting and Task Execution | 14% |
| 2 | Output Evaluation and Validation | **21%** |
| 3 | Product and Model Selection | 12% |
| 4 | Workflow Integration and Solution Design | 16% |
| 5 | Configuration and Knowledge Management | 12% |
| 6 | Governance, Risk and Responsible Use | 15% |
| 7 | Troubleshooting and Optimization | 10% |

### What the exam actually tests

The heaviest domain is not prompting, it is **judging the output**: spotting a summary that
quietly drops the exception the decision turned on, a confident answer with no source, a session
that has stopped following the framework you set at the start, and knowing when human review is not
optional. Expect scenarios about choosing between Haiku, Sonnet and Opus for a task, when to use a
Project versus a one-off chat, what belongs in project instructions versus a prompt, and which
kinds of data must never be pasted into a chat.

### Prep course

**Udemy: Claude Certified Associate (CCAO-F) exam prep** — 66 lectures, 7 quizzes, 60-question practice exam, one short video per topic, built on this domain table:
https://www.udemy.com/course/claude-associate-certification-complete-exam-prep-course/?referralCode=573675328E3CCF9C52E1
Free 2-minute overview: https://www.youtube.com/watch?v=qI5i_N5smzI

### Official documentation by domain

- Models and how to choose: https://docs.claude.com/en/docs/about-claude/models/overview
- Prompting: https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview
- Claude.ai features (Projects, Artifacts, Skills, memory, connectors): https://support.claude.com
- Responsible use and the Usage Policy: https://www.anthropic.com/legal/aup
- Defining success and evaluating output: https://docs.claude.com/en/docs/test-and-evaluate/define-success

---

## CCDV-F · Claude Certified Developer – Foundations

### Domains and weights *(exam guide v1.0, July 2026)*

| # | Domain | Weight |
|---|---|---|
| 1 | Applications and Integration | **33.1%** |
| 2 | Model Selection and Optimization | 16.8% |
| 3 | Agents and Workflows | 14.7% |
| 4 | Prompt and Context Engineering | 11.0% |
| 5 | Tools and MCPs | 10.6% |
| 6 | Security and Safety | 8.1% |
| 7 | Claude Code | 3.1% |
| 8 | Evaluation, Testing and Debugging | 2.6% |

### What the exam actually tests

One third of the exam is **applications and integration**: the Messages API, streaming, error
handling, tokens and context limits, the Batch API, prompt caching, structured output, and what to do
when a stream drops in the middle of a tool call. Model selection and optimization (cost, latency,
pinning a model version) is the second block. Claude Code and evaluation are small on paper, but
the agent and tool-use questions assume you know how they work in practice. Every item is a
scenario: "a team sees X, what should they change first?"

### Prep course

**Udemy: Claude Certified Developer (CCDV-F) exam prep** — 103 lectures, 19 quizzes, 50-question practice exam, one short video per topic, built on this domain table:
https://www.udemy.com/course/claude-developer-certification-complete-exam-prep-course/?referralCode=B6A3E536B7AD1215D394
Free 2-minute overview: https://www.youtube.com/watch?v=58khpZ2UlrA

### Official documentation by domain

- Messages API and SDKs: https://docs.claude.com/en/api/messages
- Models, pricing and context windows: https://docs.claude.com/en/docs/about-claude/models/overview and https://docs.claude.com/en/docs/build-with-claude/context-windows
- Prompt caching: https://docs.claude.com/en/docs/build-with-claude/prompt-caching
- Batch processing: https://docs.claude.com/en/docs/build-with-claude/batch-processing
- Extended thinking: https://docs.claude.com/en/docs/build-with-claude/extended-thinking
- Tool use: https://docs.claude.com/en/docs/agents-and-tools/tool-use/overview
- Model Context Protocol (MCP): https://modelcontextprotocol.io and https://docs.claude.com/en/docs/agents-and-tools/mcp
- Claude Code: https://code.claude.com/docs/en/overview (hooks, skills, MCP, headless mode, Agent SDK)
- Evaluation: https://docs.claude.com/en/docs/test-and-evaluate/define-success
- Prompt engineering: https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview

---

## CCAR-F · Claude Certified Architect – Foundations

### Domains and weights *(exam guide v1.0, July 2026)*

| # | Domain | Weight |
|---|---|---|
| 1 | Agentic Architecture and Orchestration | **27%** |
| 2 | Claude Code Configuration and Workflows | 20% |
| 3 | Prompt Engineering and Structured Output | 20% |
| 4 | Tool Design and MCP Integration | 18% |
| 5 | Context Management and Reliability | 15% |

### What the exam actually tests

Designing a system that still behaves when a tool fails or a prompt gets ignored. Orchestrator and
subagent patterns, when to parallelise and when not to, how a subagent's context is isolated, how
to design a tool's schema and description so the model uses it correctly, what goes in a
`CLAUDE.md` versus a hook versus a skill, and how to keep a long session reliable (compaction,
checkpoints, structured output with validation). One trap: the exam guide names the subagent tool
"Task", and current documentation calls it "Agent". Know both names.

### Prep course

**Udemy: Claude Certified Architect Foundations (CCAR-F) exam prep** — 31 lectures, 5 domain quizzes, 60-question timed practice exam, one short video per topic, built on this domain table:
https://www.udemy.com/course/claude-architect-foundations-complete-exam-prep-course/?referralCode=82CFCB4426395545BF28
Free 2-minute overview: https://www.youtube.com/watch?v=ZSo1W1ys1ps

### Official documentation by domain

- Building agents and orchestration: https://docs.claude.com/en/docs/agents-and-tools/overview
- Claude Code: https://code.claude.com/docs/en/overview, subagents https://code.claude.com/docs/en/sub-agents, hooks https://code.claude.com/docs/en/hooks, skills https://code.claude.com/docs/en/skills, MCP https://code.claude.com/docs/en/mcp, best practices https://code.claude.com/docs/en/best-practices
- Agent SDK: https://code.claude.com/docs/en/agent-sdk/overview
- Tool use and structured output: https://docs.claude.com/en/docs/agents-and-tools/tool-use/overview
- MCP specification (tools, resources, prompts): https://modelcontextprotocol.io/specification
- Context windows and management: https://docs.claude.com/en/docs/build-with-claude/context-windows
- Prompt engineering: https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview

---

## CCAR-P · Claude Certified Architect – Professional

### Domains and weights *(exam guide v1.0, July 2026)*

| # | Domain | Weight |
|---|---|---|
| 1 | Integration | **19%** |
| 2 | Solution Design and Architecture | 17% |
| 3 | Evaluation, Testing and Optimization | 16% |
| 4 | Governance, Safety and Risk Management | 14% |
| 5 | Stakeholder Communication and Lifecycle | 14% |
| 6 | Claude Models, Prompting and Context Engineering | 13% |
| 7 | Developer Productivity and Operational Enablement | 7% |

### What the exam actually tests

Integration, solution design and evaluation together are just over half the exam. The questions
are enterprise situations: a pipeline that runs the largest model on every step because nobody made
a model decision, PII that reaches request logs through a summarisation tool, a human review queue
so long that reviewers approve without reading, a cost model that was never checked against the
first invoice. You are asked what an architect should change, in what order, and how to explain it to
the people who approve it. Advanced level: it assumes you have shipped with an LLM API.

### Prep course

**Udemy: Claude Certified Architect Professional (CCAR-P) exam prep** — 103 lectures, 28 quizzes, 63-question timed practice exam, one short video per topic, built on this domain table:
https://www.udemy.com/course/claude-architect-professional-complete-exam-prep-course/?referralCode=D83564EB7F3969CD739E
Free 2-minute overview: https://www.youtube.com/watch?v=62j2q9yv1p8

### Official documentation by domain

- Everything listed under CCAR-F, plus:
- Model deployment platforms (Amazon Bedrock, Google Vertex AI, Microsoft Foundry): https://docs.claude.com/en/api/claude-on-amazon-bedrock, https://docs.claude.com/en/api/claude-on-vertex-ai, https://docs.claude.com/en/api/claude-on-microsoft-foundry
- Usage Policy and responsible AI: https://www.anthropic.com/legal/aup, https://www.anthropic.com/responsible-scaling-policy
- Data retention and privacy (zero data retention, PII): https://privacy.claude.com
- Evaluation and testing: https://docs.claude.com/en/docs/test-and-evaluate/define-success
- Pricing and cost optimisation: https://claude.com/pricing

---

## How to prepare (any of the four)

1. **Get the official exam guide first** (through the Partner Network registration) and copy its
   domain table into your notes. Study time follows the weights: a 33% domain gets a third of your
   hours, a 3% domain gets an afternoon.
2. **Read the documentation for the two heaviest domains end to end**, not blog summaries. The
   questions are written from the docs and from how the products behave today.
3. **Build one small thing per domain.** For CCDV-F, a script that streams a tool-use loop and
   recovers from a dropped stream. For CCAR-F, an orchestrator with two subagents and one MCP
   server. For CCAO-F, a Project with instructions and knowledge that a colleague can use. For
   CCAR-P, a one-page cost and risk model for a real workflow.
4. **Practise scenario questions under time.** 120 minutes for 53–63 items is about 2 minutes each.
   Learn to eliminate the two options that are "true but not the first thing to change".
5. **Keep a list of version-sensitive facts** (model names, context sizes, tool names like
   Task/Agent) and re-check them the week before the exam.

## Our Udemy prep courses

I built one complete prep course per certification on Udemy: every domain of the exam guide, one
short video per topic, practice quizzes per module and a full-length timed practice exam. Free
two-minute overviews are on YouTube. The course price is set on Udemy (and often discounted there);
it is separate from the exam fee above.

| Certification | Udemy course | Overview video |
|---|---|---|
| CCAO-F Associate | https://www.udemy.com/course/claude-associate-certification-complete-exam-prep-course/?referralCode=573675328E3CCF9C52E1 | https://www.youtube.com/watch?v=qI5i_N5smzI |
| CCDV-F Developer | https://www.udemy.com/course/claude-developer-certification-complete-exam-prep-course/?referralCode=B6A3E536B7AD1215D394 | https://www.youtube.com/watch?v=58khpZ2UlrA |
| CCAR-F Architect Foundations | https://www.udemy.com/course/claude-architect-foundations-complete-exam-prep-course/?referralCode=82CFCB4426395545BF28 | https://www.youtube.com/watch?v=ZSo1W1ys1ps |
| CCAR-P Architect Professional | https://www.udemy.com/course/claude-architect-professional-complete-exam-prep-course/?referralCode=D83564EB7F3969CD739E | https://www.youtube.com/watch?v=62j2q9yv1p8 |

Other languages (same slides, narration and subtitles translated):

| Course | French | Spanish | Other |
|---|---|---|---|
| CCAO-F Associate | https://www.udemy.com/course/certification-claude-associate-preparation-complete/?referralCode=25A7A1A2F5739B5A7D9A | https://www.udemy.com/course/certificacion-claude-associate-preparacion-completa/?referralCode=C56ECFA80736DCE36673 | Portuguese https://www.udemy.com/course/certificacao-claude-associate-preparacao-completa/?referralCode=7C9B5E2B3E2A4410153F · Hindi https://www.udemy.com/course/claude-associate-g/?referralCode=2ED1E8C5B39FC4E1768F · Korean https://www.udemy.com/course/claude-associate-certification-korean-exam-prep/?referralCode=F4803690ACBC896D9E59 |
| CCDV-F Developer | https://www.udemy.com/course/certification-claude-developpeur-preparation-complete/?referralCode=76802B8C5E998D806E50 | https://www.udemy.com/course/certificacion-claude-developer-preparacion-completa/?referralCode=485D749CB1E93AEA5629 | |
| CCAR-F Architect Foundations | https://www.udemy.com/course/certification-claude-architect-foundations-prepa-complete/?referralCode=9B799AE92C8F5B7B0203 | https://www.udemy.com/course/certificacion-claude-architect-foundations-curso-en-espanol/?referralCode=3B92E21E83E2C4C5CDF1 | |
| CCAR-P Architect Professional | coming soon | https://www.udemy.com/course/certificacion-claude-architect-pro-preparacion-completa/?referralCode=A37490BD9B79E0D07340 | |

YouTube channel with all the overview videos: https://www.youtube.com/@ClaudeCertPrepGuide

## Contributing

Corrections and additions are welcome, especially from people who have sat an exam: open an issue
or a pull request. Please do not post exam questions; that breaks the candidate agreement.

## Licence

Text in this repository: CC BY 4.0. Anthropic, Claude and the certification names are trademarks of
Anthropic, PBC, used here only to identify the exams.
