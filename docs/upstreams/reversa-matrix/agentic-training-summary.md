# Agentic Toolchain Training Pack

- Generated at: `2026-06-27T00:28:08.328Z`
- Target: `Fractal-Echo/claude-code-matrix`
- Profile: `agentic_toolchain`
- Sources: 9
- Source text policy: no third-party source text is copied into this pack.

## Policy Counts

| Policy | Count |
| --- | --- |
| allowlist | 1 |
| blocked | 3 |
| notice_required | 1 |
| permissive | 4 |

## Source Weights

| Repo | Import stance | Class | Weight | License evidence | Findings | Contradictions | Highest |
| --- | --- | --- | --- | --- | --- | --- | --- |
| shanraisshan/claude-code-best-practice | selective_adapt_with_attribution | permissive | 90 | MIT LICENSE in repo root | 3678 | 11 | HIGH |
| ChinaSiro/claude-code-sourcemap | reference_only_no_copy | blocked | 10 | GitHub license metadata NOASSERTION; package LICENSE says Anthropic all rights reserved/legal terms | 57383 | 1277 | HIGH |
| luongnv89/claude-howto | selective_adapt_with_attribution | permissive | 90 | MIT LICENSE in repo root | 13982 | 239 | HIGH |
| ComposioHQ/awesome-claude-skills | per_folder_allowlist_only | allowlist | 45 | GitHub license metadata NOASSERTION; selected folders have Apache-2.0 LICENSE.txt | 15156 | 328 | HIGH |
| anthropics/claude-cookbooks | selective_adapt_with_attribution | permissive | 90 | MIT LICENSE in repo root | 5817 | 417 | HIGH |
| shareAI-lab/learn-claude-code | concept_adapt_with_attribution | permissive | 90 | MIT LICENSE in repo root | 7688 | 163 | HIGH |
| claude-code-best/claude-code | reference_only_no_copy | blocked | 10 | GitHub license metadata NOASSERTION; no root license detected in local scan | 74012 | 1741 | HIGH |
| thedotmack/claude-mem | selective_adapt_with_notice_preservation | notice_required | 80 | Apache-2.0 LICENSE plus NOTICE in repo root | 15739 | 387 | HIGH |
| anthropics/claude-code | compatibility_reference_only_no_vendor | blocked | 10 | Custom Anthropic commercial terms in LICENSE.md | 6410 | 192 | HIGH |

## Use

Use `agentic-training-pack.jsonl` as a deterministic profile-training and review dataset.
Blocked/reference-only lanes may inform classifiers but must not contribute copied source text.
