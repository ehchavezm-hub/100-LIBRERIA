
<h1 align="center">👁️ Agent Reach</h1>

<p align="center">
  <strong>Let your AI agent reach the parts of the internet it can't reach on its own</strong>
</p>

<p align="center">
  Let your agent search and read X, Reddit, YouTube, XiaoHongShu…
</p>

---

## Why Agent Reach?

**Agent Reach connects your agent to the internet for real, giving it the platforms and abilities it can't reach on its own.**

CLI agents such as Claude Code, Codex, Hermes Agent and OpenClaw come with web search and page fetching, but they mostly can't reach:

- **Features that need a login**: searching XiaoHongShu notes, checking an X account's latest posts, reading job details, and more.
- **What's inside video**: YouTube and Bilibili subtitles, plus speech-to-text for YouTube videos and Xiaoyuzhou podcasts.
- **Chinese platforms**: Bilibili, XiaoHongShu, V2EX and Xueqiu, which general search covers poorly.
- **Clean structured data**: Xueqiu quotes, V2EX topics and replies, GitHub repos and issues, already cleaned up.

Agent Reach installs and tests the tools behind these platforms for you, so your agent can use them with one command:

```bash
agent-reach channels                          # which channels exist and what each can do
agent-reach youtube search "LLM agents"       # agent-reach <channel> <action> [args]
agent-reach read https://www.v2ex.com/t/123   # picks the channel from the link
```

---

## Supported Platforms

| Channel | Level | What it does | Needs |
|---|---|---|---|
| github | default | search repos, read a repo/README, read issues and PRs with comments | nothing |
| youtube | default | video info, search, subtitles, speech-to-text | nothing; speech-to-text needs a Groq or OpenAI key |
| web | default | web search, page reading (fallback) | nothing |
| v2ex | default | hot topics, nodes, topics with replies, users | nothing |
| bilibili | default | search, video info, trending, subtitles | nothing; subtitles need a login (QR scan) |
| reddit | optional | search posts, read text/comments, browse a subreddit | login |
| linkedin | optional | search jobs, read job details | public jobs need nothing; in-site search needs a login |
| xiaohongshu | optional | search notes, read text, view comments | login |
| xueqiu | optional | real-time quotes, stock search, hot posts, hot stocks | quotes need nothing; hot posts and stocks need a login |
| boss | optional | job and JD search | login |
| xiaoyuzhou | optional | podcast transcription | Groq key |
| twitter | experimental | search tweets, profiles, user tweets, threads | login |
| facebook | experimental | search, profiles | login |
| instagram | experimental | user search, profiles, user posts | login |

---

## Quick Start

Send this to your agent:

```
Install Agent Reach: https://raw.githubusercontent.com/Panniantong/Agent-Reach/main/docs/install.md
```

---

## Security

- **Read-only**: it searches and reads; it never posts, comments, likes or sends messages.
- **It never logs in for you or asks for your password.**
- **Use a secondary account** — platforms may restrict accounts used for automation.
- **Never paste keys into a chat**: run `agent-reach configure groq-key` in your own terminal.

---

## Source

GitHub: https://github.com/Panniantong/Agent-Reach  
License: MIT
