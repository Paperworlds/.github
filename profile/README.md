# Paperworlds

Text-first tools for AI development with Claude Code. Everything is a TUI, everything runs in your terminal.

The `text-` prefix is the philosophy: no GUIs, no web dashboards, no electron wrappers. If it doesn't work in a terminal, we don't ship it.

Born from building a text-based multiplayer RPG — still in private alpha.

## The tools (explore in order)

**1. [textaccounts](https://github.com/paperworlds/textaccounts)** — Manage multiple Claude Code accounts with full directory isolation.
Claude Code doesn't have profile switching. We needed separate work/personal accounts with isolated sessions, memory, and settings — not just swapped auth tokens. textaccounts treats each profile as a complete config directory.

**2. [textsessions](https://github.com/paperworlds/textsessions)** — TUI for Claude Code session management.
Browse, search, tag, and resume sessions across repos and profiles. Knows which profile was used for each session. Built for heavy Claude Code users who lose track of dozens of parallel conversations.

**3. textprompts** *(coming soon)* — Coordinate multi-agent work on single repos.
Decompose features into ordered prompt files, run them as a DAG, track progress and cost. The orchestration layer that ties it all together.

## License

Tools are released under the [Elastic License 2.0](https://www.elastic.co/licensing/elastic-license) — free to use, but not to embed or redistribute as part of other products.
