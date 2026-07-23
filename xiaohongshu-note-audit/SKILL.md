---
name: xiaohongshu-note-audit
description: >
  Audit Xiaohongshu (小红书 / RED / RedNote / XHS) note content for policy compliance
  and shadowban / traffic-throttling risk. Scans for banned words, superlative /
  absolute-claim (极限词) violations, and sensitive content, flags the risks, and
  returns actionable, compliant rewrite suggestions to avoid throttling, takedown,
  or account penalties. Use when the user wants to check a Xiaohongshu note before
  posting, do 小红书违禁词检测 / 合规审核 / 笔记预审, review 小红书文案 for compliance, or assess
  shadowban / 限流 risk. Trigger keywords: xiaohongshu, 小红书, RED, RedNote, XHS,
  compliance, audit, 审核, 违禁词, 极限词, 限流, shadowban, moderation. Requires an API key
  from wsdsocial.com.
---

# Xiaohongshu (RED) Note Compliance Audit

Audit Xiaohongshu (小红书 / RED / RedNote) note content for compliance and performance.
Checks for policy violations, banned / superlative words, shadowban (限流) risk, and
provides actionable optimization suggestions to improve visibility and pass review.

## Setup

1. Get your API key at https://ai.wsdsocial.com/skills
2. Set as environment variable: `WSD_API_KEY`

## Usage

```bash
curl -X POST "https://ai.wsdsocial.com/api/pub/skills/red-note-audit/_tool_87" \
  -H "Content-Type: application/json" \
  -H "key: ${WSD_API_KEY}" \
  -d '{
    "content": "Your full RED note content (title + body)"
  }'
```

## Parameters

| Param     | Type   | Required | Description |
|-----------|--------|:--------:|-------------|
| `content` | String | Yes      | The full RED note content including title and body text |

## Response

Returns compliance analysis, shadowban / throttling risk assessment, and optimization tips.
