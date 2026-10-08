# Persate

Connect your Persate account to research Polish legislation, parliamentary activity, public affairs, media and your accessible workspace documents. Persate returns source references for evidence-based answers. Depending on your organization's settings, the connection can also read Labs, manage alerts and preferences, and perform workspace administration with an administrator account.

![Persate](assets/logo.svg)

## Connect

Install the package in a compatible host and connect the Persate MCP server at `https://api.persate.com/mcp` using OAuth. Sign in to Persate in the browser and review the requested permissions. The organization must enable external MCP and the relevant toolsets. Write actions require separate write consent. Credentials are never entered into chat or this package.

For manual setup, add this URL in your app's remote MCP settings. [Connection guide](https://persate.com/docs/mcp).

## Skills

| Skill | Use it to |
|---|---|
| `connect-persate` | connect an account, see what the connection can reach, fix access errors |
| `polish-law` | find and read legal acts, consolidated texts, amendments and implementing regulations |
| `legislative-tracker` | follow drafts and bills from RCL through the Sejm, Senate, President and Tribunal to publication |
| `parliamentary-votes` | analyse Sejm and Senate votes, club positions and MPs' voting records |
| `stakeholder-dossier` | profile politicians, officials and institutions |
| `parliamentary-questions` | find interpellations and written questions and the government's replies |
| `sejm-debates` | find what was said in plenary sittings, committees and press conferences |
| `media-pulse` | follow public figures' posts on X, topics, events and deletions |
| `daily-briefing` | summarize a day or week in Polish politics and law, with your alert matches |
| `issue-dossier` | prepare a source-backed brief on a policy issue |
| `alerts` | review alert matches and create, edit, pause or delete alerts |
| `workspace-documents` | search, read and quote your organization's files |
| `labs-research` | explore the research Labs assigned to your organization |
| `account-settings` | change your preferences and handle notifications |
| `team-admin` | manage members, groups and invitations as an administrator |

## Example requests

- Find recent Polish legislation about telecommunications and cite the sources.
- Where is the government's draft on renewable energy in the legislative process?
- How did the parliamentary clubs vote on energy price bills in this Sejm term?
- Prepare an issue brief on the regulation of short-term rentals in Poland.
- Summarize recent events from my Persate alerts.
- Change my Persate interface language to Polish.

The available tools depend on your account and organization. This plugin cannot grant additional permissions, change account-security settings, delete files or run paid enrichment. Confirm destructive actions before execution.

## Data and support

Tool arguments are sent to Persate's API. The returned data is then processed by the AI app you connected under that app's policies. The package itself has no local database, telemetry, hooks or background jobs. Persate's existing account, access controls, audit and retention policies apply to the service. Disconnect an app in Persate Settings → MCP & AI apps to revoke its access.

[Support](https://persate.com/faq) · [Privacy](https://persate.com/documents/privacy-policy) · [Terms](https://persate.com/documents/terms-of-service)
