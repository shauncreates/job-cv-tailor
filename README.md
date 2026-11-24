# Job CV Tailor

An evidence-first Agent Skill for reviewing a CV against a real vacancy and tailoring job-application materials without inventing candidate facts.

It helps agents map requirements to evidence, surface material gaps, assess recruiter-skim readability, and write a targeted CV or application response when requested. It does not promise an ATS score or interview and does not submit applications.

## Install

### Any supported agent

With Node.js and `npx` available, install globally for the agents you use:

```sh
npx skills add shauncreates/job-cv-tailor --skill job-cv-tailor --global --agent codex claude-code antigravity gemini-cli opencode
```

Remove any `--agent` targets you do not use. To install only in the current project, omit `--global`.

The command uses the [Skills CLI](https://skills.sh/docs/cli). Its supported agent names and install paths can change; use `npx skills add --help` if a target name is rejected.

### Codex installer

In Codex, invoke `$skill-installer` and ask it to install `skills/job-cv-tailor` from `shauncreates/job-cv-tailor`. Alternatively, use the skill-installer script with:

```sh
python <path-to-skill-installer>/scripts/install-skill-from-github.py --repo shauncreates/job-cv-tailor --path skills/job-cv-tailor
```

### Manual install

Copy the `skills/job-cv-tailor` folder to a host's skill directory. Common locations include:

| Agent | User-level location |
| --- | --- |
| Codex | `$CODEX_HOME/skills/job-cv-tailor` or `~/.codex/skills/job-cv-tailor` |
| Claude Code | `~/.claude/skills/job-cv-tailor` |
| Antigravity / Gemini CLI | `~/.agents/skills/job-cv-tailor` |
| OpenCode | `~/.agents/skills/job-cv-tailor` or `~/.config/opencode/skills/job-cv-tailor` |

For workspace use, consult the host's documentation for its project-level skill directory. The same `SKILL.md` and references are portable; tool access and file generation depend on the host.

## What's included

- `skills/job-cv-tailor/SKILL.md` — concise routing and core behavior.
- `references/evidence-mapping.md` — evidence labels, gating criteria, recruiter skim risks, and an optional transparent coverage estimate.
- `references/tailoring-playbook.md` — CV, cover letter, and application-answer workflows with factual before/after examples.
- `references/document-quality.md` — file preservation, format and readability guidance, and output QA.
- `references/install-and-compatibility.md` — Agent Skills portability and official host documentation links.

## License

MIT. See [LICENSE](LICENSE).
