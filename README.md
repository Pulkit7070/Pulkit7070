<div align="center">

# Pulkit Saraf

**Full-Stack Developer · AI/ML Engineer · Blockchain Builder**

Building AI systems, developer tools, and products that ship fast and solve real problems.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077b5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/pulkit-saraf-893213290)
[![X](https://img.shields.io/badge/@PsudoKit-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/psudokit)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://psudokit.live)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:pulkitsaraf.dev@gmail.com)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@psudokit)

[![GitHub followers](https://img.shields.io/github/followers/Pulkit7070?style=for-the-badge&logo=github&label=Follow&color=181717)](https://github.com/Pulkit7070)
[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/Pulkit7070)

</div>

---

### 🔷 goto stack

`TypeScript` `JavaScript` `Python` `Java` `Rust` `Solidity` `SQL`
`React` `Next.js` `Tailwind CSS` `Framer Motion`
`Node.js` `Express` `Spring Boot`
`LangChain` `RAG` `TensorFlow` `Scikit-learn` `Agent Systems`
`Solidity` `Hardhat` `Ethers.js` `Stellar/Soroban` `Anchor (Solana)`
`PostgreSQL` `MongoDB` `Redis` `Docker` `Turborepo` `Vercel`

---

### 🔷 track record

```
30+ Hackathons  ·  8 Wins  ·  Selected for ETHGlobal, Algorand Ecosystem, ETH Mumbai
```

Currently **Full Stack Intern @ [ArmorIQ.ai](https://armorclaw.com)**  cybersecurity & AI governance infrastructure.

---

### 🔷 open source

Active contributor across CNCF and Linux Foundation projects. 19+ PRs spanning distributed tracing, authorization engines, cloud-native UI, and observability infrastructure.

```
1 Merged  ·  18 Open  ·  4 Orgs  ·  ~3,200 lines changed
```

| Project | PRs | Area |
|---|---|---|
| [jaegertracing/jaeger-ui](https://github.com/jaegertracing/jaeger-ui) | [#3905](https://github.com/jaegertracing/jaeger-ui/pull/3905) ✅ **Merged** | UI CSS / AccordionLinks fix |
| [jaegertracing/jaeger](https://github.com/jaegertracing/jaeger) | [#8574](https://github.com/jaegertracing/jaeger/pull/8574) [#8580](https://github.com/jaegertracing/jaeger/pull/8580) [#8581](https://github.com/jaegertracing/jaeger/pull/8581) [#8582](https://github.com/jaegertracing/jaeger/pull/8582) [#8583](https://github.com/jaegertracing/jaeger/pull/8583) | apiv3 gRPC/HTTP gateway · badger storage |
| [openfga/openfga](https://github.com/openfga/openfga) | [#3127](https://github.com/openfga/openfga/pull/3127) [#3130](https://github.com/openfga/openfga/pull/3130) [#3131](https://github.com/openfga/openfga/pull/3131) [#3132](https://github.com/openfga/openfga/pull/3132) [#3133](https://github.com/openfga/openfga/pull/3133) | server hardening · Postgres · typesystem |
| [meshery/meshery](https://github.com/meshery/meshery) | [#19241](https://github.com/meshery/meshery/pull/19241) [#19339](https://github.com/meshery/meshery/pull/19339) [#19485](https://github.com/meshery/meshery/pull/19485) [#19486](https://github.com/meshery/meshery/pull/19486) [#19487](https://github.com/meshery/meshery/pull/19487) [#19488](https://github.com/meshery/meshery/pull/19488) [#19489](https://github.com/meshery/meshery/pull/19489) | handler pipeline · UI/a11y · Redux · CLI |

<details>
<summary>what I actually fixed</summary>

- **jaeger-ui #3905** — corrected `AccordionLinks` CSS class name typo; added missing empty-icon colour rule. Merged by Yuri Shkuro.
- **jaeger #8574** — fixed `query.attributes` JSON parsing in HTTP gateway; attribute filters were silently discarded before this.
- **jaeger #8580** — added `spanKind` persistence to the badger operation cache; changed `map[string]uint64` → `map[tracestore.Operation]uint64`.
- **jaeger #8581** — implemented `GetDependencies` in both the gRPC handler and HTTP gateway, completing the last unimplemented apiv3 RPC.
- **jaeger #8582** — extended HTTP gateway to support `query.attributes[key]=value` bracket-notation params matching grpc-gateway URL encoding.
- **jaeger #8583** — fixed two gRPC validation paths returning `codes.Internal` instead of `codes.InvalidArgument`; added status-code assertions.
- **openfga #3127** — added 3 missing config validations in `NewServerWithOpts()` so library-mode callers get upfront errors instead of runtime panics.
- **openfga #3130** — replaced 2 `panic("unexpected userset rewrite")` calls with typed error returns in graph traversal and listusers.
- **openfga #3131** — dropped `grpc_health_probe` binary from released Docker image; Kubernetes ≥1.23 native gRPC probes remove the need for it.
- **openfga #3132** — blocked readiness until Postgres connection pool warms to `minIdleConns`; startup-only `atomic.Bool` latch prevents false NOT_SERVING under load.
- **openfga #3133** — improved error message when a tupleset relation has userset type restrictions (`InvalidTuplesetRelationTypeRestrictionError`).
- **meshery #19339** — added `ConnectionPingHandler` with per-kind registry dispatch for ad hoc connectivity checks.
- **meshery #19485** — fixed double invocation of `ErrBuildOCIImg` in `ExportModel` handler.
- **meshery #19486** — made registry bulk-action checkbox visible on hover, checked state, and keyboard focus (accessibility).
- **meshery #19487** — fixed `mesheryctl` docs generator to emit `~/.meshery/config.yaml` instead of the runner's absolute home path.
- **meshery #19488** — replaced hardcoded `alt="profile-avatar"` with owner's full name; added `rel="noopener noreferrer"` to external avatar links.
- **meshery #19489** — fixed notification center flashing stale read events by initialising filters to `STATUS.UNREAD` instead of `initial: true`.
- **meshery #19241** — corrected deprecated `word-wrap` to `overflow-wrap` in `_table.scss` while retaining the IE11 fallback.

</details>

---

### 🔷 current work

- **[Opsuna](https://github.com/Pulkit7070/opsuna)** - Generative UI engine. Natural language → production-ready React components. Solo-built.
- **[HaloAI](https://github.com/Pulkit7070/haloai)** - AI desktop assistant with blockchain-native wallet integration. Electron, Rust, Stellar/Soroban. Built with Team Kaizen.
- **[agmonverse](https://github.com/Pulkit7070/agmonverse)** - AI-powered AMM optimizer that defends against LVR attacks on Monad. *Monad Blitz Hackathon Winner 🏆*
- **[multigravity-pro](https://github.com/Pulkit7070/multigravity-pro)** - Run unlimited Antigravity IDE profiles simultaneously. Fixed critical Windows bugs, added status/link/export/import. `npm i -g multigravity-pro`
- **[get-cooked](https://github.com/Pulkit7070/get-cooked)** - Monitor AI agent usage across Claude Code, Cursor & Copilot. Alerts before rate limits, generates handoff files. `npm i -g get-cooked`
- **[NFT Marketplace](https://github.com/Pulkit7070/nft-marketplace)** - Decentralized marketplace for AI-generated space-themed NFTs. Solidity, IPFS, Ethers.js.

---

### 🔷 building from zero

I build from zero. Whether it's a generative UI engine, an AI agent that trades on-chain, a CLI tool devs actually install, or a hackathon project shipped in 36 hours  I work across the entire stack. Frontend to smart contracts to ML models to deployment. I care less about stack debates and more about shipping things people actually use.

---

### 🔷 currently exploring

- **AI agent systems** - building autonomous agents that interact with real-world systems, not just chatbots
- **Rust** - systems-level tooling, CLI performance, blockchain runtimes
- **MCP architecture** - model context protocol servers, tool orchestration, agentic workflows
- **Solana/React Native** - mobile-first crypto experiences

---

### 📊 stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Pulkit7070&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=c9d1d9" height="165" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=Pulkit7070&theme=tokyonight&hide_border=true&background=0d1117&ring=58a6ff&fire=58a6ff&currStreakLabel=58a6ff" height="165" />

</div>

<div align="center">

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pulkit7070&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9" height="150" />

</div>

---

### 🏅 leetcode

<p align="center">
  <img src="https://leetcard.jacoblin.cool/Pulkit7070?theme=dark&font=Montserrat&border=0" />
</p>

---

### 💼 work with me

I'm open to **freelance projects, sponsorships, and full-time roles** in AI/ML, full-stack, or blockchain engineering.

If you're building something ambitious  I ship fast, I've won hackathons against 500+ teams, and I care about craft.

<div align="center">

[![Sponsor on GitHub](https://img.shields.io/badge/Sponsor_My_Work-%E2%9D%A4-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/Pulkit7070)
[![Hire Me](https://img.shields.io/badge/Let's_Talk-0077b5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/pulkit-saraf-893213290)
[![Portfolio](https://img.shields.io/badge/See_My_Work-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://psudokit.live)

</div>

---

<div align="center">
  <sub>building in public as <a href="https://x.com/psudokit">@PsudoKit</a> · star a repo if it helped you ⭐</sub>
</div>
