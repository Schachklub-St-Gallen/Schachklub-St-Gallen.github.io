# CLAUDE.md

Verify site changes with `script/check`: it builds the site and checks internal links exactly as CI does, and exits non-zero on the first failure. It checks no external links; for those, `script/check --external` (run weekly by `.github/workflows/external-links.yml`). Ruby gems live in `~/gems` (`GEM_HOME`).

## Agent skills

### Issue tracker

Issues are tracked in this repo's GitHub Issues (Schachklub-St-Gallen/Schachklub-St-Gallen.github.io) via the `gh` CLI. See `docs/agents/issue-tracker.md`.

### Triage labels

Default vocabulary: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`. See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: one `GLOSSARY.md` and `docs/adr/` at the repo root (both created when first needed). See `docs/agents/domain.md`.
