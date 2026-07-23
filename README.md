# Xiaohongshu (RED) Note Compliance Audit — Agent Skill

An AI Agent Skill that audits **Xiaohongshu (小红书 / RED / RedNote / XHS)** note content for compliance and **shadowban / traffic-throttling (限流)** risk — flagging banned words, superlative/absolute-claim (极限词) violations, and sensitive content, then returning compliant rewrite suggestions.

Works with Claude Code, Cursor, Codex, OpenClaw and any agent that supports the open `SKILL.md` standard.

## What it does

Paste a full note (title + body) and it returns a compliance analysis, throttling-risk assessment, and actionable fixes so the note passes review and avoids limits, takedown, or account penalties.

## Install / use

The skill lives in [`xiaohongshu-note-audit/SKILL.md`](./xiaohongshu-note-audit/SKILL.md).

1. Get an API key at https://ai.wsdsocial.com/skills
2. Set `WSD_API_KEY` as an environment variable
3. See the SKILL.md for the request format

## Keywords

`xiaohongshu` · `小红书` · `RED` · `RedNote` · `XHS` · `compliance` · `audit` · `审核` · `违禁词` · `极限词` · `限流` · `shadowban`

---
Part of the WSD Xiaohongshu creator skill set: note generation · audit · topic planning · imitation writing.
