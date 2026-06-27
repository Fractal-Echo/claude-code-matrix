# Reversa-Matrix Upstream Evidence

This folder stores metadata-only evidence from the Reversa-Matrix Claude/Codex
upstream study. It does not vendor upstream source trees.

## Contents

- `source-sync.json` - pinned upstream repos, commits, license evidence, import
  stance, and recommended adaptation lanes.
- `TRAINING_PASS_2026-06-26.md` - Reversa training/study pass notes and
  provenance boundaries.
- `refined-scan-summary.json` - refreshed Reversa `agentic_toolchain` scan
  totals after the code-assignment classifier improvements.
- `agentic-training-summary.md` - metadata-only training pack summary.
- `agentic-training-labels.json` - evidence-category labels used for review and
  scanner tuning.
- `sha256sums.txt` - checksums for the generated metadata pack.

## Boundary

Use these files to guide local implementation and review. Do not copy from
reference-only, sourcemap-restored, no-license, or commercial-terms upstreams.
When adapting from Apache-2.0 material, preserve required NOTICE attribution.
