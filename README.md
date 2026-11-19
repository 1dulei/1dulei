# Hi, I'm Du Lei (杜雷)

**Senior Quality Engineer · Quality Architecture & AI Reliability / Evaluation**  
`Beijing, China` · [Email](mailto:a1437699690@163.com) · `8+ Years in Multi-Platform & AI Quality Engineering`

> **Quality as Code · Deterministic Guardrails for Non-Deterministic AI.**  
> Across 8+ years at **51Talk (NYSE: COE)**, **Longfor Group (HKEX: 0960)**, and **Hongben Technology**, I build deterministic release gates that catch structural regressions, silent security leaks, and LLM hallucinations *before* they reach production.

---

### Flagship Open-Source Quality Infrastructure

| System | Layer | What It Enforces | Verification |
| :--- | :--- | :--- | :--- |
| **[EvalGate](https://github.com/1dulei/evalgate)** | **LLM Evals & Red-Teaming** | Zero-dependency Python 3.11 CI gate enforcing RAG context groundedness, strict JSON Schema output contracts, snapshot prompt regression diffs (`evalgate diff`), and zero-tolerance adversarial prompt-injection / DAN / PII leak probes. | `8/8 Benchmark Green` · `0 Red-Team Leaks` |
| **[SpecGate](https://github.com/1dulei/specgate)** | **Shift-Left Diff Risk Gate** | Extracts SHA-256-signed non-executable test contracts from PRDs and audits multi-repo unified diffs (`Spring/Java`, `Android Room/Kotlin`, `Vue`) with exact `file:line` anchors for auth bypasses, status forgery, non-atomic wallet deductions, and offline sync overwrites. | `1.00 Precision & Recall` across 4 suites |
| **[TracePilot](https://github.com/1dulei/tracepilot)** | **Browser Probe & Passive Telemetry** | Selector-free Playwright intent runner recovering from hidden checkboxes, non-semantic `div` buttons, and `window.open` popups while passively sniffing `/api/` JSON payloads & `localStorage` for leaked `payPwd` hashes and `HTTP 200 + code:-1` masked failures. | `E2E Sandbox Verified` · `HTML Evidence Bundle` |

---

### Core Engineering Stack

- **AI Evaluation & Safety**: RAG Groundedness / Hallucination Metrics · JSON Schema Contract Enforcement · Prompt Regression Diffing · Adversarial Red-Teaming (Prompt Injection, Jailbreak, PII Guardrails)
- **Shift-Left & Test Architecture**: Unified Diff / AST Risk Gates · Microservice API Contracts · High-Concurrency Row-Lock & Idempotency Auditing · Weak-Network & Fault Injection
- **Automation & Telemetry**: `Python 3.11` · `TypeScript` · `Playwright` · `Pytest` · Selector-Free UI Recovery · Passive Network/Storage Sniffing · `Android ADB / Room Sync`
- **Backend Triage & CI/CD**: `Java / Spring Boot` · `MySQL` · `Redis` · `GitHub Actions / GitLab CI` · `Linux` · `Mitmproxy / Charles`

---

### Selected Field Notes

- **Deterministic Guardrails for Non-Deterministic AI**: Designing `EvalGate` to catch silent prompt regressions and red-team leaks in CI.
- **Why Textbook AI-Generated Page-Object Frameworks Rot in Two Weeks**: Replacing brittle selectors with `TracePilot` intent recovery and passive API security telemetry.
- **Blocking P0 Escapes Pre-Staging**: Turning ad-hoc LLM code review prompts into line-anchored `SpecGate` diff rules (`1.00 F1`).
