# Career Intelligence Agent v1.1
Portable research methodology and templates for Claude, ChatGPT, and later Gemini/Copilot. Default: screen 25 companies, investigate up to 5 verified open roles, balanced career strategy, preserve original resume. Scoring R40/C25/N15/P20; confidence and coverage separately. Start with SKILL.md. Follow platform-adapters/CLAUDE.md or CHATGPT.md. This package is not an autonomous service: live verification requires browsing and persistent comparisons require a previous Word report, optional snapshot or authorized storage. The default deliverable is one editable Word (.docx) report with clickable job links, plain-language scorecards, and relevant opportunity briefs. Markdown and JSON exports are optional on explicit request; the Markdown files in this package are setup instructions, not the report output. No personal data included.

## Suggested first request
"Use the Career Intelligence skill. Here is my resume [attach] and optional skills list [attach]. Target roles: [...]. Preferred geography: [...]. Screen up to 25 companies using vendor case studies and industry conference evidence plus verified job searches. Produce one editable Word report with clickable job links, clear scorecards, and up to five deep opportunity briefs. Include relevant company evidence, resume fit and gaps, interview questions, sources, and suggested next steps. Do not invent open jobs or contacts."

## Optional technical validation
Schemas use JSON Schema draft 2020-12. Sample fixture in examples/example-snapshot.json is synthetic and must never be represented as real research. Validate with: python -m json.tool research-snapshot.json (syntax only); for schema validation use a JSON Schema 2020-12 validator.

## v1.1 replacement and changes
This ZIP is a clean replacement for Career_Intelligence_Agent_v1.0.zip: the same career-intelligence/ root, exactly the same 16 paths, and no added, removed or renamed files. Replace the old folder contents with this version; no migration is needed. The archive filename changes to Career_Intelligence_Agent_v1.1.zip.

Updated files:
- SKILL.md: Word default; Markdown/JSON only on request; prior Word reports accepted for comparison.
- README.md: updated version, first request and replacement guidance.
- report-template.md: clickable job/source links, human-readable scorecards, readable Word layout and verification checks.
- interview-brief.md: present brief details within the Word report.
- platform-adapters/CLAUDE.md, CHATGPT.md, GEMINI.md and COPILOT.md: align delivery and comparison guidance with Word reports.

The other eight files are byte-for-byte unchanged: discovery-methodology.md, verification-rules.md, relationship-mapping.md, scoring-rubric.md, candidate-profile.md, both original .schema.json files, and examples/example-snapshot.json. The original schemas and synthetic example remain optional technical aids. Research methodology, verification rules, scoring weights, contact safeguards and resume safeguards are unchanged.

No particular platform is required. Live verification and Word downloads depend on available host tools. If Word generation is unavailable, the assistant must say so and provide readable content in chat. No programming is needed for ordinary use.
