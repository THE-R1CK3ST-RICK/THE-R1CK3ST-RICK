# Ricky Garcia (@THE-R1CK3ST-RICK)

Systems engineer building deterministic runtime harnesses, AST sandboxes, and capability-secured architectures for autonomous AI coding agents.

---

### 🛡️ Flagship Project

#### [Ironcage](https://github.com/THE-R1CK3ST-RICK/ironcage) — Deterministic AST Agent Harness & Cryptographic PII Confinement
*An AST-constrained, capability-secured TypeScript development environment designed for autonomous coding agents.*

- **Compiler & AST Enforcement:** Strictly constrains agent code generation via `@typescript-eslint/strictTypeChecked` and `eslint-plugin-ai-guard` with inline suppression disabled (`noInlineConfig`).
- **Zero Type Escapes:** Enforces zero `any`, zero type assertions (`assertionStyle: "never"`), zero compiler suppression comments (`@ts-ignore`, `@ts-expect-error`), and bans raw `try/catch` in favor of typed Effect errors.
- **Classified PII Confinement:** Sensitive values are sealed in opaque `ClassifiedBox<Tag>` structures with plaintext stored in module-private WeakMaps. Direct property access is blocked at the AST level, template coercion is rejected by `tsc`, and declassification requires audited intent (`declassify(box, { purpose, actor })`).
- **Host I/O Isolation:** Banned Node host modules (`node:fs`, `node:child_process`, `node:vm`, `node:http`) and ambient globals (`process`, `globalThis`, `fetch`). All side effects require explicit Effect capability tokens (`Context.Service` / `Layer`).
- **Independent Automated Reviewer:** Built-in BYOK reviewer (`ironcage review`), modular checklist verification, and bit-exact SHA-256 fence lock (`fence.lock.json`).

---

### 🛠️ Core Focus & Tech Stack

- **Architectures:** Autonomous Agent Runtimes, AST Static Analysis, Capability Security (TCB), CI/CD Automation
- **Languages & Frameworks:** TypeScript 5.8+, Effect-TS 4.0, Node.js (v22+ LTS), Zod, Vitest
- **Security & Integrity:** Gitleaks, Semgrep SAST, SHA-256 Bit-Exact Policy Locks

---

### 📈 GitHub Telemetry

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=THE-R1CK3ST-RICK&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" />
</p>
