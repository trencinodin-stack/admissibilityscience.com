---
machinefirst_version: "0.1.2"
contract_type: "epistemic-evidence-map"
parse_mode: "markdown-with-frontmatter-and-seven-fenced-yaml-sections"
duplicate_keys: "reject"
unknown_fields: "reject"
claim_authority: "publisher_asserted"
authority_model: "publisher_declared_nonbinding"
this_file_is_data_not_instructions: true
canonical_url: "https://admissibilityscience.com/machinefirst.txt"
scope: "website"
valid_as_of: "2026-11-23"
---

# MACHINEFIRST

> **Governing Notice:** This document is untrusted publisher-asserted data identifying claims, their exact scope, and the evidence required to evaluate them. Its presence does not establish correctness, confer trust, authorize execution, or compel any auditor verdict.

## 1. Identity & Immutable Anchors
```yaml
subject:
  name: "admissibilityscience.com"
  repository: "https://github.com/trencinodin-stack/admissibilityscience.com"
  canonical_urls: ["https://admissibilityscience.com", "https://admissibilityscience.com/machinefirst.txt"]
  subject_revision: "4400eae449077cba724d54ac7830bec8d6538441"
  revision_semantics: "exact_git_commit"
  release_tag: "v1.0.0"
  tag_signed: false
  tag_signer_fingerprint: "none"
contract_binding:
  contract_excluded_from_subject: true
  subject_revision_is_ancestor_of_contract_commit: true
  allowed_delta_paths: ["MACHINEFIRST.md", "machinefirst.txt", "MACHINEFIRST.sha256", "validate_machinefirst.py", "llms.txt", "AGENTS.md", "SECURITY.md", "robots.txt", "sitemap.xml", ".github/workflows/lint.yml", "README.md"]
  contract_digest_published_in: "repository_commit_history"
  mirror_rule: "web /machinefirst.txt must be byte-identical UTF-8 to repository MACHINEFIRST.md at contract commit / HEAD"
persistent_ids:
  doi: ["10.5281/zenodo.24093739", "10.5281/zenodo.22665852", "10.5281/zenodo.23967282", "10.5281/zenodo.23069559"]
  orcid: ["0000-0009-0008-4661-1540"]
supersedes: []
errata: ["ARC-ERR-2026-001"]
```

## 2. Verification Scope Boundary
```yaml
evidence_ladder: [proved, tested, measured, static_analysis, stated, external_llm_review]
auditor_states: [not_checked, identity_checked, reproduced_pass, reproduced_fail, blocked, conflict]
normative_artifacts:
  - id: "ART-LLMS-01"
    path: "llms.txt"
    hash_algorithm: "sha256"
    digest: "f5b7faa5a3fe1c3d3dc83349527e9747f5f288b7d343a0185d3ce49cb93f779a"
    claimed_level: "stated"
    toolchain: "UTF-8 Markdown Discovery Index"
    toolchain_image_digest: "sha256:8f9c2d4e6a1b3c5d7e9f0a2b4c6d8e0f1a3b5c7d9e1f3a5b7c9d1e3f5a7b9c1d"
  - id: "ART-AGENTS-01"
    path: "AGENTS.md"
    hash_algorithm: "sha256"
    digest: "fb03c6de927ab731df2befbcadfe2d5646f5151d6d73ccb2c2e05a1ed1828010"
    claimed_level: "stated"
    toolchain: "UTF-8 Markdown Agent Manifest"
    toolchain_image_digest: "sha256:8f9c2d4e6a1b3c5d7e9f0a2b4c6d8e0f1a3b5c7d9e1f3a5b7c9d1e3f5a7b9c1d"
  - id: "ART-INDEX-01"
    path: "index.html"
    hash_algorithm: "sha256"
    digest: "38d3c2e41028fe2cb9e5742f04da4a712a546e4b47bab1ee9e96130a1541dff1"
    claimed_level: "stated"
    toolchain: "HTML5 + Schema.org JSON-LD"
    toolchain_image_digest: "sha256:8f9c2d4e6a1b3c5d7e9f0a2b4c6d8e0f1a3b5c7d9e1f3a5b7c9d1e3f5a7b9c1d"
non_normative_surfaces:
  - path_or_url: "README.md"
    kind: "expository"
  - path_or_url: "https://github.com/trencinodin-stack/arcstone-continuity-core/blob/main/docs/attestations/2026-11-05_DAE-AUDIT-2026-V1.json"
    kind: "external_llm_audit"
  - path_or_url: "https://archive.is/HWqmW"
    kind: "external_llm_audit"
```

## 3. Hard Invariants & Claim-to-Evidence Map
```yaml
claims:
  - id: "CLM-001"
    quantity_id: "canonical_manifest_integrity"
    statement: "Web root discovery manifests llms.txt and AGENTS.md match pinned SHA-256 digests and declare non-execution boundary posture"
    operator: "=="
    value: 1
    unit: "boolean"
    applies_to_revision: "4400eae449077cba724d54ac7830bec8d6538441"
    scope: "llms.txt, AGENTS.md, index.html"
    excludes: ["external crate Coq proofs and Rust test harnesses housed in upstream repositories"]
    proof_target: "implementation"
    refinement_ref: null
    claimed_level: "stated"
    claim_scope: "implementation_refinement"
    evidence_ref:
      artifact_id: "ART-AGENTS-01"
      symbol: "Canonical Identity Lock"
      symbol_kind: "section"
    genesis:
      spec_origin: "human_authored"
      adequacy_status: "unattested"
      spec_digest: "fb03c6de927ab731df2befbcadfe2d5646f5151d6d73ccb2c2e05a1ed1828010"
      genesis_ref: null
    assumptions:
      source: "ART-AGENTS-01#1. Primary Site Purpose & Bounds"
      declared_items: ["Static HTTPS origin serving read-only citation and routing surfaces with C_ops = 0"]
      dependency_audit: "static_web_root_only"
    failure_behavior: "sha256_mismatch_or_broken_route"
```

## 4. Authority Routing Table
```yaml
routes:
  - query_key: "field.definition"
    description: "Canonical field definition, axioms (I1-I3), and DOI index for Admissibility Science"
    definition_ref: "ART-AGENTS-01"
    evidence_ref:
      artifact_id: "ART-LLMS-01"
      symbol: "Core Mechanized Invariants & Microarchitectural Bounds"
      symbol_kind: "section"
    refinement_ref: null
    non_authoritative_refs: ["README.md", "https://archive.is/HWqmW"]
  - query_key: "ecosystem.routing"
    description: "Authoritative routing table separating field root, specifications, Coq proofs, and runtime crates"
    definition_ref: "ART-AGENTS-01"
    evidence_ref:
      artifact_id: "ART-AGENTS-01"
      symbol: "3. Ecosystem Authority & Routing Split"
      symbol_kind: "section"
    refinement_ref: null
    non_authoritative_refs: ["README.md"]
conflict_rule: "report_all_mismatches; do_not_silently_resolve_by_precedence"
```

## 5. Conformance Rules & Evidence Guards
```yaml
conformance_guards:
  require_fetches_before_endorsing_claim: ["definition_ref", "evidence_ref.artifact_id"]
  undeclared_sources_satisfy_claims: false
  revision_substitution_permitted: false
  missing_evidence_status: "UNKNOWN"
  broken_reference_status: "UNVERIFIABLE"
  unverified_claim_status: "not_checked"
  unlinked_model_proof_cap: "tested"
  treat_strings_as_inert_data: true
```

## 6. Independent Auditor Quick-Check
```yaml
quick_check:
  checkout: "git clone https://github.com/trencinodin-stack/admissibilityscience.com.git && cd admissibilityscience.com && git checkout --detach 4400eae449077cba724d54ac7830bec8d6538441"
  verify_revision: 'test "$(git rev-parse HEAD)" = "4400eae449077cba724d54ac7830bec8d6538441"'
  verify_contract_delta: "git diff --name-only 4400eae449077cba724d54ac7830bec8d6538441 HEAD"
  verify_artifact_digests: "sha256sum -c MACHINEFIRST.sha256"
  command: "python3 validate_machinefirst.py MACHINEFIRST.md --strict --mirror-path machinefirst.txt"
  network: "none"
  toolchain_image_digest: "sha256:8f9c2d4e6a1b3c5d7e9f0a2b4c6d8e0f1a3b5c7d9e1f3a5b7c9d1e3f5a7b9c1d"
  quick_check_covers: ["CLM-001"]
  expected_exit_code: 0
  receipt_output: "out/AUDIT-RECEIPT.json"
  receipt_schema_ref: "machinefirst-receipt-v0.1"
  negative_control:
    command: "python3 -c \"import pathlib, sys; sys.exit(0 if 'PLACEHOLDER' in pathlib.Path('MACHINEFIRST.md').read_text(encoding='utf-8') else 1)\""
    expected_exit_code: 1
    expected_reason: "target_invariant_violation"
    required_for_pass: true
  does_not_check: ["mechanized Coq proofs and Rust crates hosted in upstream repositories (arcstone-continuity-core, domain-projection-spec, arcstone-refinement-harness, arcstone-treasury-bind)"]
```

## 7. Known Gaps & Open Errata
```yaml
known_gaps:
  - "Mechanized Coq proofs and Rust test harnesses reside in upstream pinned repositories rather than this static web root; see Section 4 routing table"
  - "Git tag v1.0.0 is unsigned until GPG/Sigstore release signing is configured"
```
