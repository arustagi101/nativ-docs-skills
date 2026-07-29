# Nativ Docs skills

[![skills.sh](https://skills.sh/b/arustagi101/nativ-docs-skills)](https://skills.sh/arustagi101/nativ-docs-skills)

Agent skills for creating Markdown and self-contained HTML documents that render well in [Nativ Docs](https://nativdocs.co).

## Install

For Codex:

```sh
npx skills add arustagi101/nativ-docs-skills -g -a codex -y
```

For Claude Code:

```sh
npx skills add arustagi101/nativ-docs-skills -g -a claude-code -y
```

The repository currently includes one skill:

- `nativ-docs`: supported Markdown and HTML capabilities, compatibility guidance, basic examples, and token-efficient workflows for uploading, downloading, and revising documents, and for reading their comment threads, through the Nativ Docs MCP server.

## Connect the MCP server

Codex:

```sh
codex mcp add nativ-docs-mcp --url https://mcp.nativdocs.co/mcp
```

Claude Code:

```sh
claude mcp add --transport http nativ-docs-mcp https://mcp.nativdocs.co/mcp
```

Complete the secure sign-in when your agent first connects.

## Repository structure

```text
skills/
  nativ-docs/
    SKILL.md
    agents/
      openai.yaml
```

The skill follows the open Agent Skills format and can be installed with the [`skills` CLI](https://www.skills.sh/docs/cli).
