<div align="center">

## Invariant Systems

**AI provenance infrastructure for software supply chains.**

</div>

---

### The Problem

AI tools write an increasing share of production code — but git history can't answer *which changes were AI-generated*. Trailers are inconsistent, easy to strip, and not machine-verifiable. Most AI involvement leaves no durable, tamper-evident trace.

### What We Build

AIIR (AI Integrity Receipts) is the missing provenance layer between authorship and the build pipeline. It generates deterministic, content-addressed receipts for commits with declared AI involvement and verifies them anywhere — locally, in CI, or offline — without trusting a central service.

### AIIR — AI Integrity Receipts

| | |
|:--|:--|
| **PyPI** | [`pip install aiir`](https://pypi.org/project/aiir/) |
| **GitHub Action** | [`invariant-systems-ai/aiir@v1`](https://github.com/invariant-systems-ai/aiir) |
| **GitLab CI** | One `include:` line — push and MR receipts · [GitLab Technology Partner](https://about.gitlab.com/partners/technology-partners/) |
| **VS Code** | [Extension](https://github.com/invariant-systems-ai/aiir/tree/main/extensions/vscode) — local-first commit receipts, inline verification, receipt explorer |
| **AI Assistants via MCP** | Works with Claude, Copilot, Cursor, Continue, Cline, Windsurf |
| **License** | Apache 2.0 · Zero runtime dependencies (CLI core) · Python 3.9+ |

Security posture: 2,245 tests, 100% coverage, and a public [threat model](https://github.com/invariant-systems-ai/aiir/blob/main/THREAT_MODEL.md) with 153 security controls, plus ClusterFuzzLite fuzzing and mutation testing. JSON and deterministic CBOR receipt formats. Optional Sigstore signing and PEP 740 attestations.

How it fits: AIIR fills the authorship-provenance gap *before* build-level tools (SLSA, in-toto, SCITT) kick in. See [ecosystem positioning](https://github.com/invariant-systems-ai/aiir/blob/main/docs/ecosystem.md) for the full picture.

Detection is heuristic: AIIR records what is *declared* — `Co-authored-by` trailers, bot authors, and AI-tool markers. Agent-mode sessions such as Copilot Chat, Claude Code, and Cursor Agent do not add these markers today, so those commits can still land in the `human` bucket unless the tool or user declares them explicitly. See [detection scope](https://github.com/invariant-systems-ai/aiir#detection-scope-and-limitations) for current public limits.

### Company

Invariant Systems, Inc. Delaware C-Corp. Founded 2025.

[Website](https://invariantsystems.io) · [Docs](https://invariantsystems.io/docs) · [Browser Verifier](https://invariantsystems.io/verify) · Contact: noah@invariantsystems.io

---

<sub>© 2025-2026 Invariant Systems, Inc.</sub>
