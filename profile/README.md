# Paperworlds

Text-first tools for AI development with Claude Code. Everything is a TUI, everything runs in your terminal.

The `text-` prefix is the philosophy: no GUIs, no web dashboards, no electron wrappers. If it doesn't work in a terminal, we don't ship it.

Born from building a text-based multiplayer RPG — still in private alpha.

## The tools

**01. [textworkspace](https://github.com/paperworlds/textworkspace)** — One install, one CLI for the entire text- stack.
Onboards you through the tools in dependency order, bootstraps Go binaries from GitHub releases, and exposes custom combo commands that chain actions across tools. The package manager for Paperworlds.

**02. [textaccounts](https://github.com/paperworlds/textaccounts)** `available` — Manage multiple Claude Code accounts with full directory isolation.
Claude doesn't have profile switching — we needed separate work/personal accounts with isolated sessions, memory, and settings.

**03. [textproxy](https://github.com/paperworlds/textproxy)** `optional` — Local proxy for the Claude API that captures token consumption stats.
Understand how your agentic workflows spend tokens — per session, per prompt, per model.

**04. [textsessions](https://github.com/paperworlds/textsessions)** `available` — TUI for Claude Code session management.
Browse, search, tag, and resume sessions across repos and profiles. Built for heavy users who lose track of dozens of parallel conversations.

**05. [textforums](https://github.com/paperworlds/textworkspace)** `available` — Async coordination layer for Claude Code sessions.
Post threads when you hit a cross-repo dependency, pick them up from another session. File-based, YAML threads, zero infrastructure. Ships inside textworkspace.

**06. [textread](https://github.com/paperworlds/textread)** `available` — Context-aware link reader.
URL in, relevance verdict and summary out — lensed through your stored profile and current projects. Runs as a fresh Haiku subagent per read; raw content cached locally so you can re-map without re-fetching.

**07. [textserve](https://github.com/paperworlds/textserve)** `available` — Fleet manager for MCP servers.
Start, stop, and monitor Docker-based and native MCP servers from a single CLI. Injects credentials from your password manager at runtime and auto-registers servers with Claude Code.

**08. textmap** *(coming soon)* — YAML-first knowledge graph with a Kuzu backend and MCP server.
Agents query it for protocols, open initiatives, and intent→tool mappings. Context recovery without reading prose: the graph is the source of truth, the YAML is human-authored, and `textmap sync` keeps them in step.

**09. textprompts** *(revisiting)* — Coordinate multi-agent work on single repos.
Decompose features into ordered prompt files, run them as a DAG, track progress and cost.

**10. textcombos** *(tbd)* — Community-shared workflow recipes for textworkspace.
YAML files that chain tool actions into reusable combos — install from local files, gists, or repos.

---

[paperworlds.github.io](https://paperworlds.github.io) · [Elastic License 2.0](https://www.elastic.co/licensing/elastic-license) — free to use, not to redistribute.
