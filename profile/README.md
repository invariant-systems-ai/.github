<div align="center">

## Invariant Systems

**Receipts for declared AI involvement in code changes.**

</div>

---

### What We Do

We build verifiable infrastructure for software teams using AI tools. AIIR generates tamper-evident receipts for commits with declared AI involvement so engineering, security, and audit teams can verify provenance instead of relying on screenshots or policy attestation alone.

### AIIR — AI Integrity Receipts

| | |
|:--|:--|
| **PyPI** | [`pip install aiir`](https://pypi.org/project/aiir/) |
| **GitHub Action** | [`invariant-systems-ai/aiir@v1`](https://github.com/invariant-systems-ai/aiir) |
| **GitLab CI** | One `include:` line — push and MR receipts |
| **MCP Tool** | Works with Claude, Copilot, Cursor, Continue, Cline, Windsurf |
| **License** | Apache 2.0 · Zero dependencies · Python 3.9+ |

Security posture: 1,856 tests, 100% coverage, 36 CI checks per push, public [threat model](https://github.com/invariant-systems-ai/aiir/blob/main/THREAT_MODEL.md), ClusterFuzzLite fuzzing, mutation testing. JSON and deterministic CBOR receipt formats. Optional Sigstore signing and PEP 740 attestations.

Detection is heuristic: AIIR receipts what's *declared* — `Co-authored-by` trailers, bot authors, AI-tool markers. Agent-mode sessions (Copilot Chat, Claude Code, Cursor Agent) don't add these markers today, so those commits attest as `human`. See [detection scope](https://github.com/invariant-systems-ai/aiir#detection-scope-and-limitations) for dogfood numbers.

### Company

Invariant Systems, Inc. Delaware C-Corp. Founded 2025.

Contact: noah@invariantsystems.io

---

<sub>© 2025-2026 Invariant Systems, Inc.</sub>