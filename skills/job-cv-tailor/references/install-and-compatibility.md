# Distribution and host notes

This skill uses the open Agent Skills format: a folder with `SKILL.md` and optional `references/`. It does not depend on one vendor's APIs or tool names. Hosts can still differ in automatic discovery, frontmatter support, permissions, and file-generation capability; adapt tool use to the host rather than assuming a specific tool exists.

Current host paths and procedures can change. Check the relevant official documentation before publishing updated installation guidance:

- [Agent Skills specification](https://agentskills.io/specification)
- [Codex skills](https://developers.openai.com/codex/skills/)
- [Claude Code skills](https://code.claude.com/docs/en/skills)
- [Antigravity skills](https://antigravity.google/docs/skills)
- [Gemini CLI skills](https://geminicli.com/docs/cli/skills/)
- [OpenCode skills](https://opencode.ai/docs/skills/)

The repository README provides a cross-agent installation command through the Skills CLI. Codex users can also use Codex's `$skill-installer` with this repository and the skill folder path. Do not claim that skill instructions grant tools or permissions: each host controls that separately.
