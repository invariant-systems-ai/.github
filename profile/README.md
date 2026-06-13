<div align="center">

## Invariant Systems

**Verifiable computing: receipts, proofs, and replayable evidence.**

</div>

---

### The Problem

Modern systems make claims constantly: this commit declared AI involvement, this model produced that output, this action earned that payout. Almost none of those claims come with evidence a third party can check. The most concrete case today: AI tools write an increasing share of production code, but git history can't answer *which changes were AI-generated*. Trailers are inconsistent, easy to strip, and not machine-verifiable.

### What We Build

AIIR (AI Integrity Receipts) is our first shipped product. It generates deterministic, content-addressed receipts for commits with declared AI involvement and verifies them anywhere: locally, in CI, or offline, without trusting a central service.

Public research extends the same receipt model further: inference receipts and receipted actions (attestable AI), plus evidence-first capsules in physics and mathematics, published Zenodo-first with open DOIs and explicit claim boundaries. See the [Research](https://invariantsystems.io/research) page for the linked Zenodo records and reproducibility capsules.

### AIIR | AI Integrity Receipts

| | |
|:--|:--|
| **PyPI** | [`pip install aiir`](https://pypi.org/project/aiir/) |
| **GitHub Action** | [`invariant-systems-ai/aiir@v1`](https://github.com/invariant-systems-ai/aiir) |
| **GitLab CI** | One `include:` line: push and MR receipts; [GitLab Technology Partner](https://about.gitlab.com/partners/technology-partners/) |
| **VS Code** | [Extension](https://github.com/invariant-systems-ai/aiir/tree/main/extensions/vscode): local-first commit receipts, inline verification, receipt explorer |
| **AI Assistants via MCP** | Works with Claude, Copilot, Cursor, Continue, Cline, Windsurf |
| **License** | Apache 2.0; zero runtime dependencies (CLI core); Python 3.9+ |

Security posture: 2,499 collected tests, 100% coverage, and a public [threat model](https://github.com/invariant-systems-ai/aiir/blob/main/THREAT_MODEL.md) with 150+ documented security controls, plus ClusterFuzzLite fuzzing, mutation testing, and conformance vectors. JSON and deterministic CBOR receipt formats. Optional Sigstore signing and PEP 740 attestations.

How it fits: AIIR fills the authorship-provenance gap *before* build-level tools (SLSA, in-toto, SCITT) kick in. See [ecosystem positioning](https://github.com/invariant-systems-ai/aiir/blob/main/docs/ecosystem.md) and the public [Research](https://invariantsystems.io/research) page for the current public picture.

Detection is heuristic: AIIR records what is *declared*: `Co-authored-by` trailers, bot authors, and AI-tool markers. Agent-mode sessions such as Copilot Chat, Claude Code, and Cursor Agent do not add these markers today, so those commits can still land in the `human` bucket unless the tool or user declares them explicitly. See [detection scope](https://github.com/invariant-systems-ai/aiir#detection-scope-and-limitations) for current public limits.

### Company

Invariant Systems, Inc. is a Delaware C-Corp founded in 2025.

[Website](https://invariantsystems.io) | [Docs](https://invariantsystems.io/docs) | [Research](https://invariantsystems.io/research) | [Browser Verifier](https://invariantsystems.io/verify) | Contact: noah@invariantsystems.io

---

<sub>© 2025-2026 Invariant Systems, Inc.</sub>
