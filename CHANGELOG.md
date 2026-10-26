# Changelog

## 1.0.0 — 2026-10-26

First published build: career-ops as a DeepSeek Harness plugin.

- Bundle `dsh-career-ops` with one Loader row, `career-ops`.
- Skill `career-ops`: the mode router (auto-pipeline, oferta, scan, pipeline, apply,
  pdf, cover, tracker, interview-prep, triage, patterns, upskill …), with the vendored
  System Layer as its resource base.
- Tool `career_ops`: `setup`, `scan`, `pipeline`, `tracker` (list/add/set), `liveness`,
  `report_number`, `stats`, `insight` — one implementation shared with the UI.
- Command `/career-ops`: mode menu plus live queue and tracker counts.
- Career Ops panel: sidebar row, central page with funnel cards, the applications
  tracker and a per-row status control, the pending evaluation queue, recent reports.
- `runtime/` carries career-ops 1.38.0 (`b936419e`), English modes only, with
  Playwright removed and `dsh-liveness.mjs` added — see THIRD-PARTY-NOTICES.md.
- Row config `dataRoot` is portable (`~/…` supported; falls back to
  `$CAREER_OPS_DATA_DIR` then `~/career-ops`), so one install works on every machine.
