# MAG Claude Plugins

A curated marketplace of Claude Code plugins for modern software development.

This repository packages a collection of specialized plugins for Claude Code, designed to help with frontend work, backend development, code analysis, documentation, testing, DevOps, planning, browser automation, and more. Instead of installing everything at once, you can enable only the plugins that match your project and workflow.

## Why use this repository?

Claude Code becomes much more useful when it has the right domain-specific capabilities for the work you are doing. This repo gives you a plug-and-play plugin marketplace so you can:

- accelerate frontend and UI development
- analyze and investigate large codebases
- build APIs and backend services
- generate technical documentation
- run testing and QA workflows
- coordinate multi-step work with project planning and orchestration
- automate browser-based tasks and debugging
- add specialized tools for research, databases, SEO, media, and more

## What is included?

The marketplace includes a broad set of plugins, including:

- Frontend
- Code analysis
- Bun backend
- Development workflow tools
- Testing and QA
- DevOps and release workflows
- Documentation and writing
- Planning and project coordination
- Workflow orchestration
- Browser automation
- Specialized domain plugins such as:
  - languages
  - database
  - research
  - SEO
  - media
  - blockchain
  - game
  - obsidian
  - svelte
  - and more

## Quick start

### 1) Add the marketplace

```bash
/plugin marketplace add tianzecn/myclaudecode
```

### 2) Enable the plugins you want

In your Claude Code project settings, add the plugins you need:

```json
{
  "enabledPlugins": {
    "frontend@tianzecn-plugins": true,
    "code-analysis@tianzecn-plugins": true,
    "bun@tianzecn-plugins": true
  }
}
```

You can keep the configuration in your project's `.claude/settings.json` and enable only the tools relevant to your workflow.

### 3) Start using Claude Code

Once enabled, Claude Code can help with tasks like:

- building and reviewing frontend features
- understanding a codebase
- creating or refactoring backend APIs
- generating documentation and project context
- testing and debugging changes
- coordinating engineering tasks across multiple steps

## Repository structure

```text
myclaudecode/
├── .claude-plugin/
│   └── marketplace.json
├── plugins/
│   ├── frontend/
│   ├── code-analysis/
│   ├── bun/
│   ├── development/
│   ├── testing/
│   ├── devops/
│   ├── documentation/
│   ├── planning/
│   ├── workflow/
│   ├── superpowers/
│   ├── superpowers-chrome/
│   ├── episodic-memory/
│   ├── superpowers-lab/
│   ├── superpowers-developing/
│   ├── skill-seekers/
│   ├── docs/
│   ├── languages/
│   ├── database/
│   ├── seo/
│   ├── game/
│   ├── blockchain/
│   ├── media/
│   ├── research/
│   ├── mcp/
│   ├── obsidian/
│   ├── svelte/
│   └── ...
├── ai-docs/
├── agent_docs/
├── docs/
├── tools/
│   └── claudeup/
├── AGENTS.md
├── CLAUDE.md
├── .gitignore
├── LICENSE
├── README.md
└── ...
```

## Typical plugin layout

Each plugin is designed as an independent capability bundle. A typical plugin includes metadata plus task-oriented files such as:

```text
plugins/<plugin-name>/
├── plugin.json
├── agents/
├── commands/
├── skills/
├── mcp-servers/
└── ...
```

This keeps each plugin focused and modular, instead of mixing unrelated tools into one large package.

## Recommended usage pattern

This repository is best used as a marketplace rather than as a single monolithic app.

A practical workflow is:

1. add the marketplace
2. choose only the plugins relevant to your current project
3. enable them in your workspace
4. use Claude Code to handle those tasks with the proper context

This keeps the setup lean and avoids unnecessary noise in your daily workflows.

## Environment variables

Some plugins may rely on external services or local development tools. Common examples include:

```bash
APIDOG_API_TOKEN=your-personal-token
FIGMA_ACCESS_TOKEN=your-personal-token
GITHUB_PERSONAL_ACCESS_TOKEN=your-token
CHROME_EXECUTABLE_PATH=/path/to/chrome
CODEX_API_KEY=your-codex-key
```

Keep secrets in local environment files or secure secret stores instead of committing them to the repository.

## Project docs

This repo includes both user-facing documentation and maintainer-oriented guidance:

- `README.md` — overview and usage
- `AGENTS.md` — internal contributor and AI guidance
- `CLAUDE.md` — project context for Claude Code usage
- `ai-docs/` — technical documentation
- `agent_docs/` — operational and workflow docs

## License

This project is licensed under the MIT License.

## Maintainer

- tianzecn

---

Built to help Claude Code work effectively across frontend, backend, documentation, testing, and team workflows.
