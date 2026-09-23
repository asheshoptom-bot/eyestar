# eyestar

Ashesh's daily dashboard. The live version runs on claude.ai:
https://claude.ai/artifact/CoZNd1DXCaEcG2Q9UDi1Vd

This repo is a **backup**. It holds the page source and the scheduled tasks that fill it.
It cannot be hosted on GitHub Pages as-is, because the page reads its data from claude.ai
(`claude.use('db')`). Opened anywhere else, it shows "cannot reach the data store".

## Files

| File | What it is |
|---|---|
| `eyestar.html` | Page source (republish to the URL above to restore) |
| (task prompts kept private — not in this public repo) | |

## Data collections (inside the eyestar artifact)

`projects`, `goals`, `inbox`, `library`, `briefs`, `waiting`, plus single docs
`meta/vision`, `meta/wisdom`, `signals/rx`, `signals/sales`, `signals/cash`, `signals/feeds`.

## Restoring

1. In Claude, publish `eyestar.html` to the eyestar URL, keeping capabilities `db`, `sample`,
   and `mcp` (Gmail `create_draft`, Microsoft 365 `outlook_create_reply_draft`).
2. Recreate the scheduled tasks from the private copy of the task prompts.

Cron times are in UTC. Nepal is UTC+5:45.
