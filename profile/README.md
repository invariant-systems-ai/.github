<div align="center">

## Invariant Systems

**Local-first proof infrastructure for declared AI involvement in code changes.**

</div>

---

### What We Do

We build public, verifiable infrastructure for software teams using AI tools. AIIR generates tamper-evident receipts for commits with declared AI involvement so engineering, security, and audit teams can review provenance instead of relying on screenshots or policy attestation alone.

### AIIR — AI Integrity Receipts

| | |
|:--|:--|
| **PyPI** | [`pip install aiir`](https://pypi.org/project/aiir/) |
| **GitHub Action** | [`invariant-systems-ai/aiir@v1`](https://github.com/invariant-systems-ai/aiir) |
| **GitLab CI** | One `include:` line — push and MR receipts |
| **VS Code** | [Extension](https://github.com/invariant-systems-ai/aiir/tree/main/extensions/vscode) — local-first commit receipts, inline verification, receipt explorer |
| **MCP Tool** | Works with Claude, Copilot, Cursor, Continue, Cline, Windsurf |
| **License** | Apache 2.0 · Zero dependencies · Python 3.9+ |

Security posture: 1,856 tests, 100% coverage, 36 CI checks per push, public [threat model](https://github.com/invariant-systems-ai/aiir/blob/main/THREAT_MODEL.md), ClusterFuzzLite fuzzing, and mutation testing. JSON and deterministic CBOR receipt formats. Optional Sigstore signing and PEP 740 attestations.

Detection is heuristic: AIIR records what is *declared* — `Co-authored-by` trailers, bot authors, and AI-tool markers. Agent-mode sessions such as Copilot Chat, Claude Code, and Cursor Agent do not add these markers today, so those commits attest as `human`. See [detection scope](https://github.com/invariant-systems-ai/aiir#detection-scope-and-limitations) for current public limits.

### Company

Invariant Systems, Inc. Delaware C-Corp. Founded 2025.

Contact: noah@invariantsystems.io

---

<sub>© 2025-2026 Invariant Systems, Inc.</sub>
