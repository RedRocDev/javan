# JAVAN — Product Presentation
### A visual, slide-style overview for GitHub

> **One workspace. Everything connected.**  
> Product concept — not a product launch announcement.

---

## 01 · The opportunity
### Our digital work is scattered

```mermaid
flowchart LR
 HUMAN["One person"] --> A["Mail clients"]
 HUMAN --> B["IDE / editor"]
 HUMAN --> C["Cloud drives"]
 HUMAN --> D["Web browser"]
 HUMAN --> E["AI assistants"]
 A --> F["Constant switching"]
 B --> F
 C --> F
 D --> F
 E --> F
```

Files, messages, previews and coding agents rarely share a common workspace or permission model.

---

## 02 · The thesis
### Bring the work to one canvas

```text
┌───────────────┬───────────────────────────┬────────────────┐
│ EXPLORER      │ CANVAS                    │ AI AGENT       │
│ Files         │ Code / Website / Email    │ Plan           │
│ Cloud         │ Images / Documents        │ Review         │
│ Mail          │ Split panes / Tabs        │ Execute        │
└───────────────┴───────────────────────────┴────────────────┘
```

**Javan is the workspace; modules provide capabilities.**

---

## 03 · Personalised by design
### Every install starts small

```mermaid
flowchart TD
 START["Install small Javan Core"] --> CHOOSE["Choose module cards"]
 CHOOSE --> AG["AI Agents"]
 CHOOSE --> EM["Email"]
 CHOOSE --> ST["Storage"]
 CHOOSE --> WB["Browser Canvas"]
 AG --> P["Choose provider by name & logo"]
 EM --> P
 ST --> P
 WB --> P
 P --> CONF["Configure or skip"]
 CONF --> DONE["Return to catalogue with setup status"]
 DONE --> WORK["Open Javan"]
```

Optional account creation. Skip every module and start with an empty workspace.

---

## 04 · First-class capabilities
| 👩‍💻 Developers | 🗂 Everyone | 🏢 Teams (future) |
|---|---|---|
| Editor & terminal | File explorer | Shared workspaces |
| Codex & other agents | Unified email | Multi-agent task orchestration |
| Live browser canvas | Cloud & SFTP | Approval policies |
| Diffs & tests | Search & documents | Auditable work |

---

## 05 · The Javan architecture
```mermaid
flowchart TB
 UI["Tauri + React Shell"] --> CORE["Rust Core"]
 CORE --> REG["Module Registry"]
 CORE --> AUTH["Capability & Permission Broker"]
 CORE --> DATA[("Local Data + SQLite")]
 REG --> PROVIDERS["Mail / Storage / Agents / Browser"]
 CORE <-.-> SYNC["Optional Javan Sync"]
 SYNC <-.-> TEAM["Future Javan Teams"]
```

Native core, optional integrations and a strict trust boundary.

---

## 06 · Own your experience
### Set up once. Recover anywhere.

```mermaid
sequenceDiagram
 participant O as Original laptop
 participant C as Javan Sync
 participant N as New laptop
 O->>C: Encrypted preferences & module manifest
 N->>C: Authenticate and request restore
 C-->>N: Compatible settings & module selections
 N->>N: Download verified modules
 N->>N: Restore layout & preferences
 N-->>N: Reauthenticate providers if needed
```

No forced cloud account; raw local documents and credentials are **not** included in standard settings sync.

---

## 07 · AI teams, not black boxes
```mermaid
flowchart TB
 USER["Human request"] --> ORCH["Workflow orchestrator"]
 ORCH --> DEV["Builder agent"]
 ORCH --> RESEARCH["Research agent"]
 ORCH --> MAIL["Communications agent"]
 DEV --> REVIEW["Review & validation"]
 RESEARCH --> REVIEW
 MAIL --> REVIEW
 REVIEW --> GATE{"Human approval?"}
 GATE -->|Approved| ACT["Apply / publish / send"]
 GATE -->|Rejected| ORCH
```

Human controls, resource scopes and an audit trail are part of the design.

---

## 08 · Sustainable release model
### Core, modules, optional cloud

| Layer | Distribution | Value |
|---|---|---|
| Desktop core | Signed native release | Reliable, fast local workspace |
| Modules | Verified, compatible packages | Install only what's useful |
| Javan Sync | Optional hosted service | Profiles and cross-device continuity |
| Javan Teams | Future business service | Shared work and coordinated agents |

Desktop updates and hosted service deployments remain independent.

---

## 09 · Delivery strategy
```mermaid
flowchart LR
 A["Foundation"] --> B["Module Engine"]
 B --> C["Onboarding"]
 C --> D["Codex + Canvas"]
 D --> E["Cloud + Mail"]
 E --> F["Javan Sync"]
 F --> G["Teams / Enterprise"]
```

Each stage requires an independently testable working increment; features are not represented as implemented before they exist.

---

## 10 · The long game

**Javan Desktop** for a person. **Javan Modules** for their chosen tools. **Javan Sync** across their devices. **Javan Teams** for organisations that work alongside agents.

> The product begins as a lightweight, useful workspace—not a giant app that forces everything on everyone.

---

<div align="center">

# JAVAN
**One workspace. Everything connected.**

**Open Javan Labs × RedRoc Dev**

[View roadmap](ROADMAP.md) · [Explore architecture](ARCHITECTURE.md) · [Return to README](../README.md)

</div>
