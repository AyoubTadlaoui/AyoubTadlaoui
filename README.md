<!-- ════════════════  HEADER  ════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,50:0a0a0a,100:7f1d1d&height=200&section=header&text=Atlas%20Kaisar&fontSize=54&fontColor=ffffff&fontAlignY=36&desc=Trust%20boundary%20for%20autonomous%20code&descSize=17&descAlignY=58" width="100%" alt="Atlas Kaisar" />

</div>

<!-- ════════════════  BLOCK 1 · PROOF (merged, clickable) ════════════════ -->

<div align="center">

<a href="https://github.com/bureado/awesome-software-supply-chain-security/pull/65"><img src="https://img.shields.io/badge/Listed%20in-awesome--software--supply--chain--security-1e8e3e?style=flat&labelColor=0a0a0a&logo=github&logoColor=white" alt="Listed in awesome-software-supply-chain-security (bureado PR #65, merged)" /></a>
&nbsp;
<a href="https://github.com/zed-industries/extensions/pull/6129"><img src="https://img.shields.io/badge/Accepted%20into-Zed%20extension%20registry-1e8e3e?style=flat&labelColor=0a0a0a&logo=zedindustries&logoColor=white" alt="atlas-ragnarok accepted into the Zed extension registry (PR #6129, merged)" /></a>

<sub>Both badges link to a merged PR. Click either one and verify it in one hop.</sub>

</div>

---

<!-- ════════════════  BLOCK 2 · THROUGH-LINE ════════════════ -->

I build the trust boundary for autonomous code. If you let an AI agent run `npm install` on its own, you need two things: a gate on what is allowed in, and a record of what it did that you cannot quietly edit afterward.

**npmguard** is the inbound gate. **GoLogX** is the outbound record. The same install-time gate is also being proposed upstream into the agents themselves. Single-binary, dependency-light, carried all the way to install.

> Gate the install. Record the action.

---

<!-- ════════════════  BLOCK 3 · SECURITY LINE (the brand) ════════════════ -->

## ❯ Forgeward, the security line

### [npmguard](https://github.com/AyoubTadlaoui/npmguard) · Rust

An npm install firewall for AI coding agents. It scores every package against OSV malware data, typosquat and slopsquat heuristics, and install-script analysis, then returns a verdict **before any lifecycle script runs**. Works in Claude Code, Cursor, and Codex over MCP, or as a plain CLI.

**Proof you can check:** refuses real OSV malware (for example `lodahs`, MAL-2025-25502). Ships as one Rust binary, deliberately **off npm** and installed straight from source, so the gate cannot be poisoned by the registry it guards.

![Rust](https://img.shields.io/badge/-Rust-dc2626?style=flat&labelColor=0a0a0a&logo=rust&logoColor=white)
![MCP](https://img.shields.io/badge/-MCP%20server-3b82f6?style=flat&labelColor=0a0a0a&logo=anthropic&logoColor=white)
[![Release](https://img.shields.io/badge/release-v0.1.7-3b82f6?style=flat&labelColor=0a0a0a)](https://github.com/AyoubTadlaoui/npmguard/releases/latest)

### [GoLogX](https://github.com/AyoubTadlaoui/GoLogX) · Go

A tamper-evident audit core for Go. An append-only, hash-chained, optionally Ed25519-signed `log/slog` handler. If anyone edits, deletes, reorders, or forges a line, the offline `logx verify` command catches it and reports the first entry that was touched.

**Proof you can check:** zero external dependencies. The integrity code is built on the standard library alone (`crypto/sha256`, `crypto/ed25519`, `crypto/rand`), so the thing that proves your logs were not tampered with carries no third-party code in its own trust path.

![Go](https://img.shields.io/badge/-Go-3b82f6?style=flat&labelColor=0a0a0a&logo=go&logoColor=white)
![Zero deps](https://img.shields.io/badge/-zero%20external%20deps-1e8e3e?style=flat&labelColor=0a0a0a)
[![Release](https://img.shields.io/badge/release-v0.2.1-3b82f6?style=flat&labelColor=0a0a0a)](https://github.com/AyoubTadlaoui/GoLogX/releases/latest)

---

<!-- ════════════════  BLOCK 4 · UPSTREAM / CONTRIBUTIONS ════════════════ -->

## ❯ Upstream

**Merged (landed):**

- Listed in the [awesome-software-supply-chain-security](https://github.com/bureado/awesome-software-supply-chain-security/pull/65) registry (bureado, PR #65).
- atlas-ragnarok accepted into the [Zed extension registry](https://github.com/zed-industries/extensions/pull/6129) (PR #6129).

**Proposed upstream (open, in review, not merged):**

The same install-time gate, pushed into the agents themselves as a supply-chain inspector.

- Goose: supply-chain typosquat inspector, [open PR #9642](https://github.com/block/goose/pull/9642), in review.
- OpenHands: SupplyChainSecurityAnalyzer, [open issue #3560](https://github.com/OpenHands/software-agent-sdk/issues/3560). Maintainers triaged it as an enhancement and pinged their security lead.
- Cline: [open issue #11340](https://github.com/cline/cline/issues/11340).
- Continue: [open issue #12573](https://github.com/continuedev/continue/issues/12573).
- Crush: [open issue #3090](https://github.com/charmbracelet/crush/issues/3090).

---

<!-- ════════════════  BLOCK 5 · ALSO / PERSONAL ════════════════ -->

## ❯ Also (personal, not the security line)

- **[atlas-ragnarok](https://github.com/AyoubTadlaoui/atlas-ragnarok)**: a terminal color theme plus a storm-fire GLSL shader, accepted into the Zed extension registry.
- **[GoFunAndChallenges](https://github.com/AyoubTadlaoui/GoFunAndChallenges)**: a hands-on Go course, runnable lessons and challenges, every package tested.

---

<!-- ════════════════  STACK ════════════════ -->

<div align="center">

![](https://skillicons.dev/icons?i=rust,go,swift,ts,js,react,python,docker,postgres,linux,bash,git,githubactions&theme=dark)

</div>

---

<!-- ════════════════  CONNECT ════════════════ -->

<div align="center">

<a href="mailto:atlas.kaisar@icloud.com"><img src="https://img.shields.io/badge/Email-dc2626?style=for-the-badge&logo=maildotru&logoColor=white&labelColor=0a0a0a" alt="email" /></a>
<a href="https://github.com/AyoubTadlaoui"><img src="https://img.shields.io/badge/GitHub-3b82f6?style=for-the-badge&logo=github&logoColor=white&labelColor=0a0a0a" alt="github" /></a>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7f1d1d,50:0a0a0a,100:1e3a8a&height=110&section=footer" width="100%" alt="footer" />
