# stacknil

Systems, telemetry, defensive tooling, and reviewable security artifacts.

I build small public repositories that are intentionally narrow, reproducible, and easy for a reviewer to inspect without guessing at hidden scope.

Current direction:

- systems foundations that make later telemetry and security work legible
- monitoring and detection-oriented tooling
- deterministic local workflows over black-box demos
- public-safe security writing with explicit boundaries

## Portfolio Map

| Repo | Primary signal | Start here |
| --- | --- | --- |
| [LogLens](https://github.com/stacknil/LogLens) | C++20 defensive log analysis for Linux auth evidence, with parser coverage telemetry and deterministic reports | [README](https://github.com/stacknil/LogLens/blob/main/README.md) · [reviewer path](https://github.com/stacknil/LogLens/blob/main/docs/reviewer-path.md) · [reviewer brief](https://github.com/stacknil/LogLens/blob/main/docs/reviewer-brief.md) |
| [telemetry-lab](https://github.com/stacknil/telemetry-lab) | reviewable telemetry and detection demos: windowing, dedup, bounded AI-assisted case drafting, and config-change investigation | [README](https://github.com/stacknil/telemetry-lab/blob/main/README.md) · [reviewer path](https://github.com/stacknil/telemetry-lab/blob/main/docs/reviewer-path.md) · [reviewer brief](https://github.com/stacknil/telemetry-lab/blob/main/docs/reviewer-brief.md) |
| [repo-sentinel-lite](https://github.com/stacknil/repo-sentinel-lite) | deterministic repository hygiene and lightweight secret-adjacent scanning with baselines and pre-commit integration | [README](https://github.com/stacknil/repo-sentinel-lite/blob/main/README.md) · [reviewer brief](https://github.com/stacknil/repo-sentinel-lite/blob/main/docs/reviewer-brief.md) |
| [scientific-computing-toolkit](https://github.com/stacknil/scientific-computing-toolkit) | scientific and supply-chain review infrastructure, currently led by `sbom-diff-and-risk` | [README](https://github.com/stacknil/scientific-computing-toolkit/blob/main/README.md) · [reviewer path](https://github.com/stacknil/scientific-computing-toolkit/blob/main/tools/sbom-diff-and-risk/docs/reviewer-path.md) · [reviewer brief](https://github.com/stacknil/scientific-computing-toolkit/blob/main/docs/reviewer-brief.md) |
| [systems-foundations](https://github.com/stacknil/systems-foundations) | Linux auth and networking state mini-labs with deterministic normalization and report artifacts | [README](https://github.com/stacknil/systems-foundations/blob/main/README.md) · [reviewer brief](https://github.com/stacknil/systems-foundations/blob/main/docs/reviewer-brief.md) |
| [sec-writeups-public](https://github.com/stacknil/sec-writeups-public) | sanitized security notes and reviewer-friendly publication governance | [README](https://github.com/stacknil/sec-writeups-public/blob/main/README.md) · [reviewer brief](https://github.com/stacknil/sec-writeups-public/blob/main/docs/reviewer-brief.md) |

## What Ties These Repos Together

- systems -> telemetry -> security is the main technical arc
- outputs should be inspectable by a human, not just runnable once
- documentation is part of the artifact, not cleanup after the artifact
- defensive scope and explicit boundaries matter more than inflated claims

## Publishing Discipline

Public repositories are treated as reviewable artifacts: sanitized inputs, explicit boundaries, deterministic outputs, tests where useful, and documentation that separates tool behavior from release or data claims.

AI assistance may be used for implementation and documentation drafting, but public artifacts are reviewed through tests, deterministic outputs, explicit scope boundaries, and human-maintained release notes.

## Reviewer Shortcut

If you only have 5 minutes:

1. [telemetry-lab](https://github.com/stacknil/telemetry-lab/blob/main/docs/reviewer-brief.md) - detection workflow and bounded AI-assisted analyst drafting.
2. [LogLens](https://github.com/stacknil/LogLens/blob/main/docs/reviewer-brief.md) - C++20 Linux authentication log analysis with parser observability.
3. [repo-sentinel-lite](https://github.com/stacknil/repo-sentinel-lite/blob/main/docs/reviewer-brief.md) - PyPI-published repository hygiene CLI with baselines and pre-commit support.
4. [scientific-computing-toolkit](https://github.com/stacknil/scientific-computing-toolkit/blob/main/docs/reviewer-brief.md) - SBOM/dependency risk review plus supporting scientific-data diagnostics.

## Writing

- [telemetry-lab / design notes](https://github.com/stacknil/telemetry-lab/blob/main/docs/design-notes.md)
- [systems-foundations / text processing pipelines](https://github.com/stacknil/systems-foundations/blob/main/notes/linux/text-processing-pipelines.md)
- [sec-writeups-public / SOC Fundamentals](https://github.com/stacknil/sec-writeups-public/blob/main/notes/80-blue-team/soc-fundamentals.md)

## Contact

- GitHub: [@stacknil](https://github.com/stacknil)
- Site: [stacknil.github.io](https://stacknil.github.io/)
- Email: [stacknil@proton.me](mailto:stacknil@proton.me)
