# stacknil

Security-minded systems builder working on telemetry, monitoring, defensive tooling, automation, and constrained AI-assisted workflows.

## What I do

I build small, practical projects that sit between systems, security, and operational data.

My current direction is shaped around:

- Linux, networking, and core systems understanding
- detection-oriented security engineering
- telemetry, monitoring, and signal processing
- public-safe technical writing and sanitized security notes
- AI-assisted workflows with explicit human verification, scope boundaries, and no autonomous response claims

## Selected Work

### [LogLens](https://github.com/stacknil/LogLens)
C++20 defensive log analysis CLI for Linux authentication logs.

- parses both legacy syslog and `journalctl --output=short-full` style input
- normalizes authentication evidence before detection
- applies configurable rule-based detections
- emits deterministic Markdown and JSON reports
- includes CI, CodeQL, and repository hardening

### [telemetry-lab](https://github.com/stacknil/telemetry-lab)
A four-demo public repository for deterministic, reviewable, local file-based telemetry and detection workflows.

- `telemetry-window-demo`: sliding-window telemetry analytics and rule-based alerts
- `ai-assisted-detection-demo`: deterministic detection and grouping with constrained LLM summarization
- `rule-evaluation-and-dedup-demo`: before/after dedup, cooldown behavior, and suppression reasons
- `config-change-investigation-demo`: risky config changes with bounded evidence correlation
- latest milestone: [`v0.6.0`](https://github.com/stacknil/telemetry-lab/releases/tag/v0.6.0)
- reviewer packs: [`ai-assisted-detection-demo`](https://github.com/stacknil/telemetry-lab/releases/download/v0.4.0/telemetry-lab-reviewer-pack-v0.4.0.zip) and [`config-change-investigation-demo`](https://github.com/stacknil/telemetry-lab/releases/download/v0.6.0/telemetry-lab-reviewer-pack-v0.6.0.zip)

### [sec-writeups-public](https://github.com/stacknil/sec-writeups-public)
Public, sanitized security write-ups from authorized labs and training platforms.

- focused on methodology, reasoning, and reusable patterns
- designed for safe publication instead of copy-paste exploitation
- organized as a maintainable public knowledge base
- includes publication boundaries and sanitization rules

## Current Focus

- building finished defensive / telemetry-oriented tools
- strengthening Linux and networking depth
- improving public project presentation and documentation quality
- preparing an English-first technical portfolio for international applications

## Working Style

- clear scope over inflated claims
- reproducibility over demos that only work once
- defensive and public-safe by default
- documentation, testing, and repository hygiene matter

## Notes

Most repositories here are learning-driven engineering artifacts:
small enough to finish, structured enough to review, and honest about their boundaries.

## Contact

- GitHub: [@stacknil](https://github.com/stacknil)
