# stacknil

**Systems-oriented defensive security tooling for Linux evidence,
product-security workflows, and software supply-chain review.**

I build narrow, local-first tools that turn system, repository, and dependency
evidence into deterministic artifacts, bounded findings, and reproducible
review paths.

Current focus:

- Linux authentication and process/socket evidence, parser coverage, and telemetry bridges
- deterministic detection and investigation workflows with schema-validated provenance
- repository and dependency review gates with redaction, baselines, SARIF, and release evidence

Stable release evidence: [LogLens v0.6.0](https://github.com/stacknil/LogLens/releases/tag/v0.6.0) · [telemetry-lab v1.2](https://github.com/stacknil/telemetry-lab/releases/tag/v1.2) · [repo-sentinel-lite v0.8.1](https://github.com/stacknil/repo-sentinel-lite/releases/tag/v0.8.1) · [scientific-computing-toolkit v1.1.0](https://github.com/stacknil/scientific-computing-toolkit/releases/tag/v1.1.0) · [systems-foundations v0.3.0](https://github.com/stacknil/systems-foundations/releases/tag/v0.3.0)

## Portfolio Map

| Repo | Primary signal | Start here |
| --- | --- | --- |
| [LogLens](https://github.com/stacknil/LogLens) | C++20 Linux authentication evidence analysis with explicit parser uncertainty, multi-episode detections, and deterministic report contracts | [README](https://github.com/stacknil/LogLens/blob/main/README.md) · [reviewer path](https://github.com/stacknil/LogLens/blob/main/docs/reviewer-path.md) · [reviewer brief](https://github.com/stacknil/LogLens/blob/main/docs/reviewer-brief.md) |
| [telemetry-lab](https://github.com/stacknil/telemetry-lab) | five local detection and investigation workflows with schema-validated artifacts, run manifests, and bounded AI assistance | [README](https://github.com/stacknil/telemetry-lab/blob/main/README.md) · [reviewer path](https://github.com/stacknil/telemetry-lab/blob/main/docs/reviewer-path.md) · [reviewer brief](https://github.com/stacknil/telemetry-lab/blob/main/docs/reviewer-brief.md) |
| [repo-sentinel-lite](https://github.com/stacknil/repo-sentinel-lite) | PyPI-published product-security guardrail with redacted output, baseline-backed scans, changed-file gates, and fail-closed configuration | [README](https://github.com/stacknil/repo-sentinel-lite/blob/main/README.md) · [reviewer brief](https://github.com/stacknil/repo-sentinel-lite/blob/main/docs/reviewer-brief.md) |
| [scientific-computing-toolkit](https://github.com/stacknil/scientific-computing-toolkit) | release-facing SBOM and dependency review with JSON, Markdown, and SARIF artifacts plus conservative policy and provenance evidence | [README](https://github.com/stacknil/scientific-computing-toolkit/blob/main/README.md) · [reviewer path](https://github.com/stacknil/scientific-computing-toolkit/blob/main/tools/sbom-diff-and-risk/docs/reviewer-path.md) · [reviewer brief](https://github.com/stacknil/scientific-computing-toolkit/blob/main/docs/reviewer-brief.md) |
| [systems-foundations](https://github.com/stacknil/systems-foundations) | four Linux evidence mini-labs, including a versioned bridge from process/socket diffs to telemetry-lab-compatible JSONL | [README](https://github.com/stacknil/systems-foundations/blob/main/README.md) · [reviewer brief](https://github.com/stacknil/systems-foundations/blob/main/docs/reviewer-brief.md) |
| [sec-writeups-public](https://github.com/stacknil/sec-writeups-public) | public-safe security pattern library with maturity, provenance, sanitization, and publication governance enforced in CI | [README](https://github.com/stacknil/sec-writeups-public/blob/main/README.md) · [reviewer brief](https://github.com/stacknil/sec-writeups-public/blob/main/docs/reviewer-brief.md) |

## What Ties These Repos Together

- Linux evidence -> telemetry and detection -> product and supply-chain security review
- evidence -> normalization -> bounded judgment -> auditable artifact
- schemas, compatibility notes, provenance, and release evidence are part of the tool contract
- defensive scope and explicit non-goals matter more than inflated claims

## What I'm Building Toward

Monitoring, detection, and product-security engineering where defensive tools
must be explainable, compatible with developer workflows, and reproducible by
another engineer. The next depth comes from stronger Linux evidence handling,
clearer telemetry contracts, and practical repository and supply-chain gates,
not from expanding project count.

## Publishing Discipline

Public repositories are treated as reviewable artifacts: sanitized inputs, explicit boundaries, deterministic outputs, tests where useful, and documentation that separates tool behavior from release or data claims.

AI assistance may be used for implementation and documentation drafting, but public artifacts are reviewed through tests, deterministic outputs, explicit scope boundaries, and human-maintained release notes.

Near-term focus: deepen evidence contracts, compatibility tests, and consumer reproduction across the existing portfolio.

## Reviewer Shortcut

If you only have 5 minutes:

1. [LogLens](https://github.com/stacknil/LogLens/blob/main/docs/reviewer-path.md) - Linux auth evidence, parser uncertainty, and detection episode semantics.
2. [telemetry-lab](https://github.com/stacknil/telemetry-lab/blob/main/docs/reviewer-path.md) - five local detection workflows, schema contracts, and provenance manifests.
3. [repo-sentinel-lite](https://github.com/stacknil/repo-sentinel-lite/blob/main/docs/reviewer-brief.md) - PyPI product-security guardrail with redaction, baselines, and changed-file gates.
4. [scientific-computing-toolkit](https://github.com/stacknil/scientific-computing-toolkit/blob/main/tools/sbom-diff-and-risk/docs/reviewer-path.md) - v1.1 SBOM/dependency review with SARIF, policy, and provenance evidence.

## Review Questions

Focused external review is welcome on:

- parser coverage: are supported, skipped, and unsupported inputs visible?
- provenance: can a reviewer trace generated artifacts to their committed inputs and configuration?
- compatibility: are schema, report, and baseline changes explicit and tested?
- policy boundary: does each warning say what it proves and what it does not prove?

Please open a focused issue in the relevant repository and include the exact
command, artifact, or sanitized example under review. Use synthetic or
public-safe inputs only.

## Writing

- [LogLens / parser uncertainty as evidence](https://github.com/stacknil/LogLens/blob/main/docs/case-study-parser-uncertainty-as-evidence.md)
- [telemetry-lab / evidence pipeline contract](https://github.com/stacknil/telemetry-lab/blob/main/docs/evidence-pipeline-contract.md)
- [systems-foundations / 408 to Linux security](https://github.com/stacknil/systems-foundations/blob/main/notes/408-to-linux-security.md)
- [sec-writeups-public / SBOM policy warning](https://github.com/stacknil/sec-writeups-public/blob/main/patterns/supply-chain/sbom-policy-warning.md)

## Contact

- GitHub: [@stacknil](https://github.com/stacknil)
- Site: [stacknil.github.io](https://stacknil.github.io/)
- Email: [stacknil@proton.me](mailto:stacknil@proton.me)
