# Research Drop Template

Save each finished research pass as its own file in this folder, named:

    YYYY-MM-DD-topic-slug.md

Example: `2026-08-05-lower-guk-named-mobs.md`

Don't edit `research-log.md` directly — the Integration Agent appends to
it automatically when it processes your drop. Don't save into
`processed/` — that's where files get moved to after they've been
applied.

One topic per file. If you're researching three zones, that's three
files, not one bundled file — it keeps each pass traceable to a single
commit.

---

## Required format (copy this exactly)

```
## Research Pass: [YYYY-MM-DD]
**Topic:** [zone / class / mechanic being researched]
**Sources checked:** [URL, URL, URL]

### Confirmed
- [fact] — source: [URL], confirmed [YYYY-MM-DD]
- [fact] — source: [URL], confirmed [YYYY-MM-DD]

### Unconfirmed / Do Not Publish
- [item] — reason: [conflicting sources / no source / stale data / etc.]

### Notes for Build Agent
[which site sections this affects — loot-codex.html, spell-upgrades.html,
or a new page; new content vs. update to existing content; anything
ambiguous that needs a human call on placement]
```

## Rules

- Every "Confirmed" fact needs a source URL and a confirmation date. No
  source → it goes in Unconfirmed, no exceptions, even if you're
  confident from memory or a prior pass.
- If two sources conflict, put it in Unconfirmed with both sources
  listed and the conflict named as the reason — don't silently pick one.
- Source priority: eqlwiki.com (primary) > everquestlegends.com
  (official) > eqlegends.wiki / eqlegendsdb.com (cross-check only) >
  EverQuest Legends Compendium Google Sheet (cross-check only, unknown
  authorship). Never backfill EQL data from classic EverQuest / Project
  1999 — EQL's multiclassing, +10 gear upgrades, and mote-fed spell
  upgrades don't exist in classic EQ, so P99/classic knowledge doesn't
  transfer.
- Nothing changed since the last pass on a topic? Say so plainly:

  ```
  ## Research Pass: [date]
  **Topic:** [topic]
  **Sources checked:** [URLs]

  ### Confirmed
  No changes from prior pass ([date of prior pass]).

  ### Unconfirmed / Do Not Publish
  (none)

  ### Notes for Build Agent
  No action needed.
  ```

  An empty pass is a valid, useful result — don't pad it out to look
  more productive.

## What happens after you drop a file

A scheduled task polls this folder every 30 minutes. When it finds your
file, it applies each Confirmed item as a targeted diff to the relevant
HTML (never a full-file rewrite), skips everything in Unconfirmed,
appends a summary to `research-log.md`, commits, pushes, and moves your
file into `processed/`. If something doesn't clearly map to an existing
section, it's held back and flagged as needing manual placement rather
than guessed at.
