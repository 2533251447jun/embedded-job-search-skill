# Acceptance Checklist

Use this checklist after every edit. Every item must be PASS before release.

## Legal and Source Boundary

- [ ] `LICENSE` keeps Santiago Fernández de Valderrama copyright.
- [ ] `LICENSE` keeps Greson Kwan copyright.
- [ ] `LICENSE` keeps `Copyright (c) 2026 2533251447jun`.
- [ ] Copyright lines appear in the required order.
- [ ] Project name is `embedded-job-search-skill`, not `career-ops` or `JobOK`.
- [ ] `NOTICE.md` explains the `career-ops` TRADEMARK boundary.
- [ ] `NOTICE.md` states this is not an official source-project version.
- [ ] `NOTICE.md` says no special permission was granted by source authors.
- [ ] JobOK audit result states: 未发现额外 NOTICE/TRADEMARK 文件。
- [ ] No source project logo, visual asset, brand identity, endorsement, certification, or official wording is used.

## Skill Structure

- [ ] `SKILL.md` frontmatter is valid YAML.
- [ ] `name` is `embedded-job-search-skill`.
- [ ] `description` starts with `Use when`.
- [ ] `description` stays under system limits.
- [ ] `SKILL.md` uses a Skill Router architecture.
- [ ] Heavy embedded knowledge is in `references/`, not fully copied into `SKILL.md`.
- [ ] `templates/` contains reusable forms.
- [ ] `examples/` contains embedded-specific scenarios.
- [ ] `tests/pressure-scenarios.md` exists.

## Required Content

- [ ] Embedded role routing covers STM32/MCU firmware.
- [ ] Embedded role routing covers embedded testing.
- [ ] Embedded role routing covers hardware debug/joint debug.
- [ ] Embedded role routing covers IoT.
- [ ] Embedded role routing covers industrial control/data acquisition.
- [ ] Embedded role routing covers BSP/Linux/driver.
- [ ] Embedded role routing covers vehicle communication testing.
- [ ] Embedded role routing covers medical/instrument/security/access/consumer electronics.
- [ ] RTOS route exists.
- [ ] BSP/Linux route exists.
- [ ] IoT route exists.
- [ ] Industrial control route exists.
- [ ] Embedded testing route exists.
- [ ] Vehicle testing/function-safety boundary reminders exist.
- [ ] Hardware debug template exists.
- [ ] Project bullet evidence tracing exists.
- [ ] Interview follow-up generation rules exist.
- [ ] Market note includes date and web-verification boundary.

## Truthfulness and Safety

- [ ] `needs_proof` is defined and used.
- [ ] `not_allowed` is defined for fabrication and platform abuse.
- [ ] The skill forbids fabricated education.
- [ ] The skill forbids fabricated internships or work history.
- [ ] The skill forbids fabricated projects.
- [ ] The skill forbids fabricated mass production.
- [ ] The skill forbids fabricated customers or commercial results.
- [ ] The skill forbids automatic applications.
- [ ] The skill forbids automatic private messages.
- [ ] The skill forbids platform-rule bypassing.
- [ ] The skill does not write “了解” as “熟练”.
- [ ] The skill does not turn course projects into company projects.
- [ ] The skill does not turn simple UART into protocol-stack ownership.
- [ ] The skill does not turn wiring into hardware design.

## Non-Copying Review

- [ ] Prose is rewritten and organized for embedded job search.
- [ ] README structure is not copied from source projects.
- [ ] JobOK text is not keyword-replaced into embedded wording.
- [ ] `career-ops` mode names are not copied as project modes.
- [ ] The project is not a generic job-search Skill with embedded keywords sprinkled in.

## File Completeness

- [ ] `SKILL.md`
- [ ] `README.md`
- [ ] `LICENSE`
- [ ] `NOTICE.md`
- [ ] `CHANGELOG.md`
- [ ] `examples/embedded-profile-example.md`
- [ ] `examples/jd-analysis-example.md`
- [ ] `examples/resume-project-example.md`
- [ ] `examples/interview-followups-example.md`
- [ ] `examples/apply-message-example.md`
- [ ] `templates/embedded-profile-template.md`
- [ ] `templates/jd-analysis-template.md`
- [ ] `templates/project-bullets-template.md`
- [ ] `templates/hardware-debug-template.md`
- [ ] `templates/interview-followups-template.md`
- [ ] `templates/application-message-template.md`
- [ ] `references/embedded-role-keywords.md`
- [ ] `references/embedded-technical-map.md`
- [ ] `references/embedded-market-notes.md`
- [ ] `references/embedded-interview-topics.md`
- [ ] `references/evidence-status-guide.md`
- [ ] `tests/pressure-scenarios.md`
- [ ] `tests/acceptance-checklist.md`
