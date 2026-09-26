# admissibilityscience.com — Canonical Root Repository

> **Master Anchor:** `A-77-DELTA-SHIELD-LOCKED`  
> **Sponsoring Entity:** Arcstone Adaptive Science Systems, Inc.  
> **Principal Architect:** Jesse Tuohy ([ORCID: 0009-0008-4661-1540](https://orcid.org/0009-0008-4661-1540))  
> **Master Suite DOI:** [10.5281/zenodo.22665852](https://doi.org/10.5281/zenodo.22665852)  
> **Foundational Field DOI (CORE02):** [10.5281/zenodo.22969294](https://doi.org/10.5281/zenodo.22969294)

---

## System Overview

This repository contains the production code for **[admissibilityscience.com](https://admissibilityscience.com/)**, the canonical field root for Admissibility Science. 

The site serves as a machine-first, dual-consumer routing and definition surface for human researchers, AI indexers, vector crawlers, and LLM agentic gateways. It establishes the mathematical axioms, runtime invariants ($I_1–I_3$), order-theoretic join-semilattice mechanics ($L, \sqcup$), and hardware clamps ($C_{\text{ops}} = 0$, $S_{\text{max}} \le 4096\text{B}$, $\tau_{\text{override}} \le 11.99\text{ms}$) governing pre-ingress proposal evaluation.

---

## Repository Structure (4-File Surface)

This site is engineered with zero framework overhead ($C_{\text{ops}} = 0$) and zero dynamic build dependencies:

| File | Purpose & Consumer |
| :--- | :--- |
| **`index.html`** | Human presentation surface, dark-mode UI, and embedded Schema.org JSON-LD machine graph. |
| **`AGENTS.md`** | Raw machine-readable specification and routing rules for AI agents, crawlers, and MCP clients. |
| **`robots.txt`** | Web crawler permissions explicitly allowing indexers to crawl `/` and `/AGENTS.md`. |
| **`sitemap.xml`** | Standard XML indexing graph mapping canonical endpoints for rapid vector ingestion. |

---

## Ecosystem Routing Hierarchy

To prevent conceptual conflation, this root surface enforces strict cross-domain separation:

* **Field Root (`admissibilityscience.com`):** Pure theoretical discipline, mathematical axioms, and paper citations.
* **Epistemic Registry ([arcstonescienceauthority.org](https://arcstonescienceauthority.org/)):** Registered fields, domain definitions, laws, and mathematical primitives.
* **Industrial Runtime ([arcstoneos.com](https://www.arcstoneos.com/)):** eBPF micro-kernels, bounded edge membranes, and production deployment substrates.
* **Protocol Contract ([`arcstone-spec-epistemic-01`](https://github.com/trencinodin-stack/arcstone-spec-epistemic-01)):** Locked upstream Epistemic Network Protocol (ENP) master specification.
* **Reference Substrate ([`arcstone-continuity-core`](https://github.com/trencinodin-stack/arcstone-continuity-core)):** `#![no_std]` Rust implementation of Subsystem 9 execution invariants.

---

## Edge Deployment

Deployed globally via **Cloudflare Pages**:
* **Build Command:** *(none / static)*
* **Build Output Directory:** `/`
* **CDN Posture:** Sub-millisecond global DNS resolution with edge SSL acceleration.
