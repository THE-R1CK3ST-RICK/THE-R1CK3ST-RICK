# Ricky Garcia (@THE-R1CK3ST-RICK)

Tech enthusiast with a systematic brain building cool AI agent tooling for fun.

I enjoy exploring what happens when you give autonomous coding agents hard boundaries: zero type escapes, isolated host capabilities, and strict deterministic fences.

---

### 🛡️ Flagship Project

#### [Ironcage](https://github.com/THE-R1CK3ST-RICK/ironcage) — Deterministic AST Agent Harness & Cryptographic PII Confinement
*An AST-constrained, capability-secured TypeScript harness designed to keep autonomous coding agents honest.*

- **Why I built it:** AI agents love taking shortcuts (`any`, `// @ts-ignore`, ambient `console.log`, and `process.env` leaks). Ironcage puts an AST "electric fence" around agent-authored code.
- **Compiler & AST Enforcement:** Strictly constrains code generation via `@typescript-eslint/strictTypeChecked` and `eslint-plugin-ai-guard` with inline suppressions disabled (`noInlineConfig`).
- **Zero Type Escapes:** Enforces zero `any`, zero type assertions (`assertionStyle: "never"`), zero compiler suppression comments, and typed Effect errors instead of raw `try/catch`.
- **Classified PII Confinement:** Sensitive values are sealed into opaque `ClassifiedBox<Tag>` structures with plaintext stored in module-private WeakMaps. Direct property access is blocked at the AST level, template coercion is rejected by `tsc`, and declassification requires audited intent (`declassify(box, { purpose, actor })`).
- **Host I/O Isolation:** Banned ambient globals (`process`, `globalThis`, `fetch`) and Node host modules (`node:fs`, `node:http`). All I/O requires explicit Effect capability tokens (`Context.Service` / `Layer`).
- **Independent Automated Reviewer:** Built-in BYOK reviewer (`ironcage review`), modular checklist verification, and bit-exact SHA-256 fence lock (`fence.lock.json`).

---

### 🛠️ Tech I Enjoy Working With

- **Agent Tooling & Runtimes:** Autonomous Agent Harnesses, AST Static Analysis, Capability Security (TCB), CI/CD
- **Languages & Libraries:** TypeScript, Effect-TS, Node.js, Zod, Vitest
- **Security & Integrity:** Gitleaks, Semgrep SAST, SHA-256 Bit-Exact Policy Locks

---

### 📈 GitHub Telemetry

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=THE-R1CK3ST-RICK&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" />
</p>
