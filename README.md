# Ricky Garcia (@THE-R1CK3ST-RICK)

Tech enthusiast with a systematic brain building cool software and AI agent tooling for fun.

I build across several domains—from gamified co-op productivity and VR fitness architectures to deterministic AI agent runtimes. **Ironcage** is my first public open-source project.

---

### 🛡️ First Public Release: [Ironcage](https://github.com/THE-R1CK3ST-RICK/ironcage)
*A deterministic AST harness and cryptographic PII sandbox designed to keep autonomous AI coding agents honest.*

- **Why I built it:** AI coding agents love cutting corners (`any`, `@ts-ignore`, empty `catch {}`, and leaking secrets into console logs). Ironcage puts an AST "electric fence" around agent-authored code.
- **Compiler & AST Constraints:** Enforces strict typing with `@typescript-eslint/strictTypeChecked` and `eslint-plugin-ai-guard` with inline suppressions disabled (`noInlineConfig`).
- **Zero Type Escapes:** Enforces zero `any`, zero type assertions (`assertionStyle: "never"`), zero compiler suppression comments, and typed Effect errors instead of raw `try/catch`.
- **Classified PII Confinement:** Sensitive values are sealed into opaque `ClassifiedBox<Tag>` structures with plaintext stored in module-private WeakMaps. Direct property access is blocked at the AST level, template coercion is rejected by `tsc`, and declassification requires audited intent (`declassify(box, { purpose, actor })`).
- **Host I/O Isolation:** Banned ambient globals (`process`, `globalThis`, `fetch`) and Node host modules (`node:fs`, `node:http`). All I/O requires explicit Effect capability tokens (`Context.Service` / `Layer`).
- **Independent Automated Reviewer:** Built-in BYOK reviewer (`ironcage review`), modular checklist verification, and bit-exact SHA-256 fence lock (`fence.lock.json`).

---

### 🧪 Other Active Lab Projects (In Development)
- **VRFJ Mainframe:** Core React codebase, Keytel math engine, and UI architecture for VR Fitness Journey.
- **Calendar Co-Op:** Cross-platform shared calendar and gamified quest/task tracker featuring dual-timelines and solo/co-op hubs.

---

### 🧰 Tech I Enjoy Building With
- **Ecosystems & Runtimes:** TypeScript, Node.js (v22+ LTS), React, Effect-TS, Zod
- **Agent Tooling & ASTs:** AST Static Analysis, ESLint Flat Config, Autonomous Agent Harnesses
- **Integrity & Security:** Gitleaks, Semgrep SAST, SHA-256 Bit-Exact Policy Locks

---

### 📈 GitHub Telemetry

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=THE-R1CK3ST-RICK&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" />
</p>
