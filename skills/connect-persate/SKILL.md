---
name: connect-persate
description: Connect a Persate account through OAuth, explain which Persate tools and data areas this connection can use, or fix a connection that is refused, expired, read-only or missing tools. Use when the user wants to set up Persate, asks what Persate can do here, or a Persate tool returns an access or permission error.
---

# Connect Persate

Persate's MCP server is `https://api.persate.com/mcp`. Connecting starts the host app's OAuth flow: the user signs in to Persate in the browser, completes two-factor authentication and approves the connection. A chat message cannot connect the account. Never ask for passwords, authenticator codes or tokens in the conversation.

## What a connection can reach

Access is the intersection of the data areas (toolsets) the organization enabled, the user's existing Persate permissions and what the user approved on the consent screen.

| Toolset | Covers |
|---|---|
| Legislation | acts, government drafts, Sejm prints, legislative processes, votes, Constitutional Tribunal, parliamentary questions |
| Media | Sejm recordings and speeches, X posts and Media events, stakeholder profiles |
| Alerts | the user's alerts and their matches; creating and editing alerts |
| Workspace | documents visible to the user, preferences, notifications |
| Labs | research Labs assigned to the organization |
| Research | cohort studies over public sources (`analysis_start`, `analysis_status`, `analysis_results`, `analysis_read`, `analysis_cancel`) and `resources_read`, which reads many returned `resource_uri` values in one call |
| Administration | members, groups and invitations, for administrators only |

Changes need write consent (`mcp:write`) and an organization set to read and write; so does starting or cancelling a study, which also needs assessments enabled for the organization. A connection approved as read-only, or before a toolset was enabled, must be reconnected to gain the new access.

## Steps

1. If Persate tools are available, name the tool families you can see and what they allow. Do not call data tools only to demonstrate them.
2. If a tool reports `access_denied`, `tool_not_available` or a missing scope, show the message and explain the likely cause using the table above.
3. Point the user to Persate Settings → MCP & AI apps to review or revoke connections. Organization administrators choose the toolsets, read or write mode and permitted apps there.
4. A revoked or expired connection needs a new sign-in through the host app.

Do not try to change organization policy, re-register the client or use other tools to get around a refusal.

Setup guide: https://persate.com/docs/mcp
