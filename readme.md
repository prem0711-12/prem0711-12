<img width="1000" height="563" alt="slack-support-assistant-demo" src="https://github.com/user-attachments/assets/b2749e1d-4df8-4d10-b484-1781dc4a5fc9" />
<h1 align="center">Hi, I'm Prem 👋</h1>
<h3 align="center">Technical / Application Support Engineer</h3>
<p align="center">Production Support · Incident Investigation · Root Cause Analysis · SQL · Automation · AI-Assisted Tooling</p>

<p align="center">
  <img src="https://img.shields.io/badge/Focus-Application%20Support-2d3748?style=flat-square&labelColor=1a202c&color=0d9488" alt="Focus: Application Support"/>
  <img src="https://img.shields.io/badge/Target-L2%20Support%20Roles-2d3748?style=flat-square&labelColor=1a202c&color=0d9488" alt="Target: L2 Support Roles"/>
  <img src="https://img.shields.io/badge/Based%20in-Ahmedabad%2C%20India-2d3748?style=flat-square&labelColor=1a202c&color=475569" alt="Based in Ahmedabad, India"/>
</p>

---

I work in production-facing technical support for SaaS platforms — investigating customer-impacting incidents, analysing logs and databases, troubleshooting integrations, and working with engineering teams to drive issues toward resolution.

My day-to-day involves understanding what happened in production, identifying the root cause, validating impact, and communicating technical findings clearly to both technical and non-technical stakeholders. I'm also interested in improving repetitive support workflows through automation and AI-assisted tooling — not as a developer, but as someone who understands the workflow and uses AI to help build practical prototypes around it.

---

## 🧭 What I Do

**Production & Application Support**
Incident investigation and troubleshooting · Root Cause Analysis (RCA) · Production issue monitoring · Customer-impacting issue investigation · Incident documentation · Engineering escalation and coordination

**Technical Investigation**
SQL / MySQL · GCP & log analysis · API troubleshooting · Postman · Firebase · Database investigation · Basic cloud and application troubleshooting

**Automation & AI-Assisted Workflows**
Support workflow automation · AI-assisted investigation and documentation · Workflow prototyping · Using AI tools to design and build practical support tooling

---

## 🧩 How I Approach Production Problems

```mermaid
flowchart TD
    A[Customer Report] --> B[Understand the Impact]
    B --> C[Reproduce / Investigate]
    C --> D[Check Logs & Data]
    D --> E[Identify Root Cause]
    E --> F[Validate the Finding]
    F --> G[Document the Resolution]
    G --> H[Communicate Clearly]
```

This is the same structured thinking behind every project below — each one started as a real support problem, not a coding exercise.

---

## 🗺️ The Story Behind My Projects

```mermaid
flowchart LR
    A[Real Support<br/>Experience] --> B[Problem<br/>Observed]
    B --> C[Workflow<br/>Idea]
    C --> D[AI-Assisted<br/>Prototype]
    D --> E[Testing]
    E --> F[Lessons<br/>Learned]
```

I don't build software for its own sake. Each project below started with something I noticed in support work — a repetitive task, a slow handoff, an assignment process that could be more consistent — and I used AI-assisted development to turn that observation into a working prototype: I define the problem, workflow, logic, and testing direction; AI assists with implementation.

---

## 🔒 Featured Project

### Slack Support Assistant — AI-Assisted Support Workflow Prototype

<p>
  <img src="https://img.shields.io/badge/Repository-Private-2d3748?style=flat-square&labelColor=1a202c&color=64748b" alt="Repository: Private"/>
  <img src="https://img.shields.io/badge/Status-Prototype%20%2F%20Experimental-2d3748?style=flat-square&labelColor=1a202c&color=0d9488" alt="Status: Prototype / Experimental"/>
  <img src="https://img.shields.io/badge/Production%20Use-No-2d3748?style=flat-square&labelColor=1a202c&color=475569" alt="Production Use: No"/>
</p>

| | |
|---|---|
| **Problem** | Support teams handling incoming Slack conversations often assign requests manually, with no consistent check on who's actually available before a conversation lands on their queue. |
| **Approach** | Prototype a workflow where new Slack conversations are detected automatically, routed to an available engineer using round-robin logic, and tracked through acknowledgement and response — with AI assisting the engineer's response drafting, not replacing their judgment. |

**Workflow**

```mermaid
flowchart TD
    A[Customer submits request in Slack] --> B[Conversation created]
    B --> C[Check engineer availability<br/>Slack presence]
    C --> D[Round-robin assignment]
    D --> E[Customer acknowledgement sent]
    E --> F[Engineer reviews conversation]
    F --> G[AI-assisted response draft generated]
    G --> H{Engineer decision}
    H -->|Edit / Regenerate| G
    H -->|Approve| I[Response sent as assigned engineer]
    I --> J[Conversation state tracked]
```

**What I experimented with**
- Excluding engineers from assignment based on real-time Slack presence, not just a static schedule
- Keeping AI in a drafting/assist role — every response is reviewed and approved by the engineer before sending, never auto-sent
- Tracking conversation and acknowledgement state through the full lifecycle, not just at creation

**Demo**

<img width="1000" height="563" alt="slack-support-assistant-demo" src="https://github.com/user-attachments/assets/205679d7-a5ff-4158-bb83-be09806d3278" />

*Screen recording of the prototype: a new conversation comes in, availability is checked, an AI-suggested reply is generated, and the engineer approves and sends it.*

**Example system output**

<details>
<summary>Sanitized log excerpt (click to expand)</summary>

```text
Engineer availability check:
Prem       presence=active   -> eligible
Aditya     presence=away     -> excluded

New Conversation
Assigned Engineer: Prem
Status: ASSIGNED

Conversation Acknowledged
Acknowledged By: Prem
Status: ACKNOWLEDGED
```

</details>

**What I learned**
Building this clarified how much of "support automation" is really about designing the *decision logic* — who's eligible, when to escalate, when to hand control back to a human — rather than the AI generation step itself, which is the easy part.

**Repository:** Private — implementation available on request
**Focus:** Support workflow design · Automation · Slack workflows · AI-assisted tooling

---

## 🗂️ Other Projects

<table>
<tr>
<td width="50%" valign="top">

**🔎 Production Support Case Studies**
*Problem:* Practising realistic production-support scenarios end to end.
*Approach:* Documented incident investigations covering RCA, SQL investigation, log analysis, and API troubleshooting, written up the way I'd document a real ticket.
*What I learned:* Structuring the investigation trail matters as much as finding the root cause — a finding nobody can follow isn't useful yet.

![Repository: Public](https://img.shields.io/badge/Repository-Public-2d3748?style=flat-square&labelColor=1a202c&color=0d9488)

</td>
<td width="50%" valign="top">

**🗄️ SQL Support Case Studies**
*Problem:* Application support issues are often really data issues.
*Approach:* SQL investigation scenarios modelled on real support situations — joins, filtering/aggregation, transaction analysis, log/data correlation.
*What I learned:* Most "SQL skill" in support work is really about knowing which question to ask the data first.

![Repository: Public](https://img.shields.io/badge/Repository-Public-2d3748?style=flat-square&labelColor=1a202c&color=0d9488)

</td>
</tr>
<tr>
<td width="50%" valign="top">

**📊 SQL Training Dashboard**
*Problem:* Wanted a more practical way to practise and present SQL analysis than one-off scripts.
*Approach:* Small project to structure SQL practice and surface results in a usable format.
*What I learned:* Presenting a query's output well is part of the job, not an afterthought.

![Repository: Public](https://img.shields.io/badge/Repository-Public-2d3748?style=flat-square&labelColor=1a202c&color=0d9488)

</td>
<td width="50%" valign="top">

**🎯 Job Search Tracker**
*Problem:* Needed a consistent way to manage my transition toward L2 Application Support roles.
*Approach:* Tracking system for target companies, applications, roles, ATS coverage, status, and follow-ups.
*What I learned:* Treating a job search like an incident queue — status, ownership, follow-up — actually keeps it manageable.

![Repository: Public](https://img.shields.io/badge/Repository-Public-2d3748?style=flat-square&labelColor=1a202c&color=0d9488)

</td>
</tr>
</table>

---

## 📈 Current Learning / Career Direction

I'm focused on moving into L2 Application Support / Production Support roles, particularly with European and German companies — deepening my incident investigation, RCA, and SQL work while continuing to explore how AI-assisted tooling can practically support (not replace) technical support teams.

---

## ✉️ Contact

📧 [premrathod1416@gmail.com](mailto:premrathod1416@gmail.com)
💼 [linkedin.com/in/premrathodtech](https://linkedin.com/in/premrathodtech)
