# Agentic Upstream Goodies

This fork tracks Claude/Codex agent-tooling ideas through a Reversa-Matrix
source-ingestion pass. The purpose is to identify compatible patterns worth
adapting while keeping license and provenance boundaries explicit.

Detailed pinned evidence lives in Reversa-Matrix:

- `docs/upstreams/claude-code-matrix/source-sync.json`
- `docs/upstreams/claude-code-matrix/TRAINING_PASS_2026-06-26.md`

This repo also keeps metadata-only copies of the Reversa study under
`docs/upstreams/reversa-matrix/` so release/review work can inspect provenance,
scan counts, labels, and checksums without vendoring upstream source trees.

## Import Policy

| Source | Policy | Useful Patterns |
| --- | --- | --- |
| `shanraisshan/claude-code-best-practice` | MIT, selective adaptation | Claude settings, hooks, skills, subagent workflow checklists |
| `luongnv89/claude-howto` | MIT, selective adaptation | Beginner docs, slash commands, skills, subagents, hooks, plugins |
| `anthropics/claude-cookbooks` | MIT, selective adaptation | Cookbook audit, CI review, managed-agent examples |
| `shareAI-lab/learn-claude-code` | MIT, concept adaptation | Skill loading, memory, agent teams, worktree isolation |
| `thedotmack/claude-mem` | Apache-2.0, NOTICE required | Persistent context architecture, hook lifecycle, memory/search boundaries |
| `ComposioHQ/awesome-claude-skills` | Per-folder allowlist only | Skill taxonomy, packaging checks, MCP builder ideas |
| `ChinaSiro/claude-code-sourcemap` | Reference only | Sourcemap/restored-source detection and import-risk warnings |
| `claude-code-best/claude-code` | Reference only | Idea radar only; cross-check against licensed or official sources |
| `anthropics/claude-code` | Compatibility reference only | Official plugin layout, settings examples, hook/security patterns |

## Recommended Integration Order

1. Add an upstream-attribution check to docs/release workflows.
2. Convert safe Claude settings and hook policy ideas into local checklists.
3. Add a Reversa-generated source-sync manifest to future architecture reviews.
4. Build a small memory/context provenance layer before importing any larger
   daemon or semantic-search architecture.
5. Treat sourcemap-restored, decompiled, no-license, and commercial-terms source
   as classifier/reference material only.

## Reversa Profile

Use Reversa's `agentic_toolchain` profile for future scans of this repo and
related upstreams:

```bash
node /path/to/Reversa-Matrix/bin/reversa.js scan \
  --project-root /path/to/claude-code-matrix \
  --profile agentic_toolchain \
  --out reversa_agentic_out
```

The profile classifies instruction files, skills, hooks, permissions, provider
routing, memory/context injection, subagent orchestration, worktree isolation,
MCP/plugin surfaces, attribution requirements, and proprietary-source import
risk.

Latest refined scan of this repo:

- Findings: `16347`
- Contradictions: `0`
- Patch candidates: `1`
- Remaining candidate: the intentional migration TODO in `cli/entrypoints.py`
