# stacknil

I build **C++ and Python tools for Linux evidence, repository hygiene, and
software supply-chain review**. My focus is systems programming and defensive
security: making inputs, decisions, and output contracts inspectable.

Start with the code below. The [portfolio website](https://stacknil.github.io/)
adds selected engineering cases and a five-minute review route.

## Start with the code

| Project | Engineering focus | Reproduce / inspect | Tagged release |
| --- | --- | --- | --- |
| [LogLens](https://github.com/stacknil/LogLens) | C++20 auth-log parsing, coverage telemetry, detection episodes, Markdown/JSON reports | [Reviewer path](https://github.com/stacknil/LogLens/blob/main/docs/reviewer-path.md) | [v0.6.0](https://github.com/stacknil/LogLens/releases/tag/v0.6.0) |
| [telemetry-lab](https://github.com/stacknil/telemetry-lab) | Five local detection/investigation demos, schema contracts, and run manifests | [Operator reproduction](https://github.com/stacknil/telemetry-lab/blob/main/docs/operator-reproduction.md) | [v1.2](https://github.com/stacknil/telemetry-lab/releases/tag/v1.2) |
| [repo-sentinel-lite](https://github.com/stacknil/repo-sentinel-lite) | Heuristic repository scans, redaction, reviewed baselines, and changed-file gates | [Consumer setup](https://github.com/stacknil/repo-sentinel-lite/blob/main/docs/consumer-minimal-setup.md) | [v0.8.1](https://github.com/stacknil/repo-sentinel-lite/releases/tag/v0.8.1) |
| [scientific-computing-toolkit](https://github.com/stacknil/scientific-computing-toolkit) | SBOM/dependency diffing with JSON, Markdown, SARIF, local policy, and optional provenance | [SBOM reviewer path](https://github.com/stacknil/scientific-computing-toolkit/blob/main/tools/sbom-diff-and-risk/docs/reviewer-path.md) | [v1.1.0](https://github.com/stacknil/scientific-computing-toolkit/releases/tag/v1.1.0) |

Supporting work:

- [systems-foundations](https://github.com/stacknil/systems-foundations): four
  saved-evidence Linux mini-labs, including a process-diff-to-JSONL adapter.
  [Process workflow and tests](https://github.com/stacknil/systems-foundations/blob/main/projects/linux-process-observe/README.md)
  · [tagged v0.3.0](https://github.com/stacknil/systems-foundations/releases/tag/v0.3.0).
- [sec-writeups-public](https://github.com/stacknil/sec-writeups-public):
  [security pattern cards](https://github.com/stacknil/sec-writeups-public/tree/main/patterns)
  with supporting lab notes and Python publication checks.

Tag links describe released versions. The source and tests linked on main can
include subsequent work. Detection demos remain local labs; scanner and policy
outputs support review without certifying that a system or package is safe.

## Cross-repository engineering

[Saved process evidence → telemetry aggregation](https://github.com/stacknil/telemetry-lab/blob/de542cb3cadba776c8e759f786152f9222fdfdb7/docs/case-study-process-evidence-to-telemetry.md)
connects systems-foundations to telemetry-lab at pinned public commits.
[PR #96](https://github.com/stacknil/telemetry-lab/pull/96) merged after v1.2.
The article reports successful ingestion and aggregation with zero alerts;
it does not establish detection efficacy. Code, fixtures, and producer goldens
are public; full execution receipts remain privately retained.

## Selected upstream contributions

Authored PRs, with status checked **20 October 2026**. Contribution scope is the
linked diff; the upstream projects retain their own authorship and review process.

- **Open** — [microsoft/sarif-tools #115](https://github.com/microsoft/sarif-tools/pull/115):
  preserve the full result description after a rule ID, with regression tests.
- **Open** — [microsoft/sarif-tools #117](https://github.com/microsoft/sarif-tools/pull/117):
  contextual filter-configuration diagnostics and advisory zero-match warnings.
- **Open** — [ossf/pvtr-github-repo-scanner #513](https://github.com/ossf/pvtr-github-repo-scanner/pull/513):
  return `NeedsReview` when check-suite/run evidence is incomplete, with Go regressions.

## Selected writing

- [LogLens: parser uncertainty as evidence](https://github.com/stacknil/LogLens/blob/main/docs/case-study-parser-uncertainty-as-evidence.md)
- [telemetry-lab: evidence pipeline contracts](https://github.com/stacknil/telemetry-lab/blob/main/docs/evidence-pipeline-contract.md)
- [systems-foundations: Linux notes](https://github.com/stacknil/systems-foundations/tree/main/notes/linux)

## Publishing and review

Public work uses sanitized fixtures, explicit input/output contracts, and
reproduction commands. AI assistance may be used for implementation and drafting;
tests, artifact inspection, and human review determine what is published.

Focused issues are welcome on parser coverage, schema compatibility, provenance,
or policy decisions. Include the exact command and a sanitized example in the
relevant repository.

## Contact

[GitHub / stacknil](https://github.com/stacknil) ·
[Website](https://stacknil.github.io/) ·
[stacknil@proton.me](mailto:stacknil@proton.me)
