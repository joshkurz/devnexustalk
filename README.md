# Unlocking Engineering Productivity with IDE-Based Coding Agents

**DevNexus 2026** | Josh Kurz

> What if the tools you already have could handle the work you dread?

## View the Slides

**[Live presentation](https://joshkurz.github.io/devnexustalk/)**

Use arrow keys to navigate. Press `S` to open speaker notes.

## What This Talk Covers

This talk follows one engineer's Monday morning -- 4 PR reviews, 2 critical CVEs, and a feature due Friday -- and shows how IDE-based coding agents can help clear every notification before lunch.

**The tools:**
- **VS Code Copilot** -- prompt files (`.prompt.md`), `@github` agent, Agent Mode
- **Claude Code** -- `/review`, `/security-review` skills, subagents
- **Atlassian Rovo MCP** -- connecting Jira tickets directly to your agent workflow

**The workflow for each task:**
| Notification | VS Code | Claude Code |
|---|---|---|
| 4 PRs waiting | `/review-code` prompt file | `/review` skill |
| CVE-2026-1847 (SQL injection) | `/review-code focus=security` | `/security-review` skill |
| FEAT-4921 (rate limiter, due Friday) | Agent Mode + Atlassian Rovo MCP | Claude + MCP |

**The message:** These tools make it easy to generate code. The hard part is shipping *quality*. Every workflow shown is human-in-the-loop -- the agent handles the mechanical work, you provide the judgment.

## Running Locally

```bash
npm install
npm start
```

Opens at [http://localhost:8080](http://localhost:8080).

## Tech Stack

- [Reveal.js](https://revealjs.com/) via [Asciidoctor reveal.js](https://docs.asciidoctor.org/reveal.js-converter/latest/)
- Slides written in AsciiDoc (`slides.adoc`)
- Custom CSS for notification card styling (`custom.css`)

## Resources Mentioned in the Talk

- [VS Code Copilot Prompt Files](https://code.visualstudio.com/docs/copilot/customization/prompt-files)
- [VS Code Custom Instructions](https://code.visualstudio.com/docs/copilot/customization/custom-instructions)
- [Claude Code Skills & Slash Commands](https://docs.anthropic.com/en/docs/claude-code)
- [Atlassian Rovo MCP Server](https://github.com/atlassian/atlassian-mcp-server)
- [GitHub MCP Server](https://docs.github.com/en/copilot/how-tos/provide-context/use-mcp/set-up-the-github-mcp-server)

## License

MIT
