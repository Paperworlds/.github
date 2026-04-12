# Paperworlds

We're building a text-based multiplayer RPG — currently in **private alpha** (a free-time passion project).

Along the way we had to build internal tools to manage multi-agent AI development with Claude Code. These turned out to be useful on their own, so we're sharing them.

## The tools (explore in order)

**1. [textaccounts](https://github.com/paperworlds/textaccounts)** — Manage multiple Claude Code accounts with full directory isolation.
Claude Code doesn't have profile switching. We needed separate work/personal accounts with isolated sessions, memory, and settings — not just swapped auth tokens. textaccounts treats each profile as a complete config directory.

**2. [textsessions](https://github.com/paperworlds/textsessions)** — TUI for Claude Code session management.
Browse, search, tag, and resume sessions across repos and profiles. Knows which profile was used for each session. Built for heavy Claude Code users who lose track of dozens of parallel conversations.

**3. textprompts** *(coming soon)* — Coordinate multi-agent work on single repos.
Decompose features into ordered prompt files, run them as a DAG, track progress and cost. The orchestration layer that ties it all together.

## License

Tools are released under the [Elastic License 2.0](https://www.elastic.co/licensing/elastic-license) — free to use, but not to embed or redistribute as part of other products.
