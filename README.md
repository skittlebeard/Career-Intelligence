# Career Intelligence Agent v1.0
Portable research methodology and templates for Claude, ChatGPT, and later Gemini/Copilot. Default: screen 25 companies, investigate up to 5 verified open roles, balanced career strategy, preserve original resume. Scoring R40/C25/N15/P20; confidence and coverage separately. Start with SKILL.md. Follow platform-adapters/CLAUDE.md or CHATGPT.md. This package is not an autonomous service: live verification requires browsing and persistent comparisons require snapshots. No personal data included.

## Suggested first request
"Use the Career Intelligence skill. Here is my resume [attach] and optional skills list [attach]. Target roles: [...]. Preferred geography: [...]. Screen up to 25 companies using vendor case studies and industry conference evidence plus verified job searches. Produce one ranked report, up to five deep briefs, and a JSON snapshot. Do not invent open jobs or contacts."

## Validation
Schemas use JSON Schema draft 2020-12. Sample fixture in examples/example-snapshot.json is synthetic and must never be represented as real research. Validate with: python -m json.tool research-snapshot.json (syntax only); for schema validation use a JSON Schema 2020-12 validator.
