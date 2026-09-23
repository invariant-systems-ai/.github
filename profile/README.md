<div align="center">

## Invariant Systems

**Dependable computation. Find hidden failures. Keep the evidence.**

</div>

---

### The Problem

Computers can return wrong answers without crashing. ECC protects against covered data errors, but a command can arrive intact and still belong to the wrong operation. Silent computational failures have been documented in production by [Google](https://research.google/pubs/cores-that-dont-count/) and [Meta](https://engineering.fb.com/2021/02/23/data-infrastructure/silent-data-corruption/).

### Our First Product

Our first product in development is an FPGA hardware integrity supervisor that complements ECC. Our supervisor is designed to check relationships defined with domain experts and preserve evidence when those checks fail. We start with a paid evaluation of one command or data path: agree on the checks, inject faults, and compare the evidence with your current approach. Prototype stage. Building toward a supported, licensable component.

In one recorded FPGA test, an injected fault raised a mismatch while redundancy kept the output correct. Controlled prototype result. Complete hardware integration and production qualification remain ahead. [Explore the technology & evidence](https://invariantsystems.io/#evidence)

### The Same Problem, Across Layers

We're pursuing the same reliability problem through software checks, formal reasoning, and hardware supervision. Proofs establish properties within their model and assumptions. FPGA results cover specific tested conditions. Hardware correspondence, broader fault coverage, and production qualification remain separate work. Technical evaluation packets are available under NDA.

### Public Research

Records on Zenodo:

- *The exact fourth-vector feasibility wall of the canonical MUB triple in dimension six*: [10.5281/zenodo.20670933](https://doi.org/10.5281/zenodo.20670933) · [`mub6-wall-atlas`](https://github.com/invariant-systems-ai/mub6-wall-atlas)
- *Inference Receipts: Lightweight Cryptographic Commitment Chains for Auditable Generative AI*: [10.5281/zenodo.18888733](https://doi.org/10.5281/zenodo.18888733)
- *Receipted Actions: A Reproducible Audit Capsule for Rewarded-Action Payout Adjudication*: [10.5281/zenodo.20008485](https://doi.org/10.5281/zenodo.20008485)
- *An Evidence-First Reproducibility Capsule for NISQ Benchmarking*: [10.5281/zenodo.19954163](https://doi.org/10.5281/zenodo.19954163) · [`research-evidence-log`](https://github.com/invariant-systems-ai/research-evidence-log)
- *Order-Dependent Breakdown of the Fricke-Vogt Invariant Under Higher-Order n-Bonacci Recursions*: [10.5281/zenodo.18882504](https://doi.org/10.5281/zenodo.18882504)

### Company

Invariant Systems is a Delaware C-corporation (USA).

[Website](https://invariantsystems.io) | [About](https://invariantsystems.io/about.html) | [Discuss an FPGA evaluation](mailto:noah@invariantsystems.io?subject=FPGA%20supervisor%20evaluation) | Contact: noah@invariantsystems.io

---

<sub>© 2026 Invariant Systems</sub>
