# EQL Research Log

Running record of research passes applied to the site. Each entry
corresponds to a file processed from `eql/_data/research-drops/`.

## 2026-08-05 — Mob & loot table + Planes of Power

**Applied by:** Integration Agent, from two compiled reference docs handed off directly in chat (`eql-mob-and-loot-table.md`, `eql-planes-of-power.md`), sourced from the 2026-08-05 research pass.

**loot-codex.html:**
- Cross-checked ~150 named-mob rows from the mob & loot table against existing zone data; added the ~45 that were genuinely new (not already covered) to 10 existing zones: Nektulos Forest, Crushbone, Befallen, Najena, Permafrost, Estate of Unrest, Solusek's Eye, Castle Mistmoore, Lower Guk, Nagafen's Lair. New mobs are tagged under a "2026-08-05 Research Pass" region per zone since the source data didn't include sub-region/location detail — kept separate from hand-placed geographic regions rather than guessing placement.
- Added 4 zones that didn't exist in the codex yet: South Ro, North Ro, Ocean of Tears, High Keep (24 mobs total).
- Extended the card renderer to support a generic multi-item `drops` list for mobs with 3+ untagged drops (previous schema only supported a common/rare pair).
- Zone count updated 16 → 32 in UI copy.
- No existing mob entries were modified or removed.

**New page — eql/planes-of-power.html:**
- Full reference for Plane of Hate, Fear, and Sky: access mechanics, named mobs/bosses, loot tables, quests, Sky's island chain and 16 class-quest chains.
- Linked from eql/index.html as a third card.
- Open follow-ups from the source doc (unitemized Innoruuk/Maestro loot, unconfirmed epic-quest components in Fear, unresearched Sky random-drop table) carried forward as a flagged section rather than guessed at.

Source: eqlwiki.com, per the underlying 2026-08-05 research-drop files.

## 2026-08-05 — BIS gear guide

**Applied by:** Integration Agent, from `eql-bis-gear-guide.md` handed off directly in chat, sourced from the 2026-08-05 research pass.

**New page — eql/bis-gear.html:**
- Best-in-slot gear reference for all 16 classes, by slot: standard BIS/Alternates tables for Warrior, Paladin, Shadow Knight, Ranger, Bard, Rogue, Cleric, Druid, Shaman; unranked Options tables for the four pure casters (Necromancer, Wizard, Magician, Enchanter) per the wiki's own "not strict BIS" disclaimers; Monk's blended Plane-of-Sky-reward + quest-track table (raid-tier is a documented gap); explicit content-gap callouts for Berserker and Beastlord (no data exists on eqlwiki.com — not backfilled from classic EQ/P99 per source instructions).
- Cross-class notes carried over verbatim (shared caster itemization, the "first item = BIS" convention and which classes it applies to, ammo-slot gap, +10/Exaltation caveat).
- Linked from eql/index.html as a fourth card; card grid adjusted to a clean 2x2 layout.

Source: eqlwiki.com, per the underlying 2026-08-05 research-drop files.

## 2026-08-07 — Bard/Shadow Knight/Druid trio guide

**Applied by:** Integration Agent, from two docs handed off directly in chat: `eql-trio-bard-shadowknight-druid.md` (2026-08-07 pass, original synthesis) and `eql-bis-no-restrictions.md` (2026-08-05 pass, explicitly unconfirmed premise).

**New page — eql/trio-bard-shadowknight-druid.html:**
- Trio overview, full Stances/Invocations tables + definitions + role-based loadout recommendations, per-class ability kits (Bard/Shadow Knight/Druid), gear guidance, race/Primary-class eligibility + leveling zone hypothesis, and an open-gaps section.
- This doc is explicitly labeled by its own source as "original synthesis... not a transcription of an existing authoritative guide" — published as a build guide, not folded into the Confirmed-only reference pages (loot-codex, planes-of-power, bis-gear). All inline hedges (classic-EQ-analogy flags, "working hypothesis, not yet fully confirmed" on the leveling route) preserved verbatim.
- **Handled a cross-pass conflict:** the 2026-08-07 trio doc reports the armor-restriction question as "now resolved" (item access is just a per-item Class: tag, verified on 2 Chest items) — this narrows/supersedes the premise the older 2026-08-05 `eql-bis-no-restrictions.md` explicitly flagged as unconfirmable. Rather than silently picking one, the page presents the resolved finding first, then carries the older doc's pooled cross-class item table forward as reference material with an explicit note reframing it in light of the newer finding, plus the original doc's own caveats (uncited fan-site source, recommendation to use eqlegendstools.com/bis-gear/ for a real numeric answer) preserved.
- Linked from eql/index.html as a 5th card; grid moved to a 3-column layout that wraps cleanly.

Source: eqlwiki.com, class/race pages, item data — per the 2026-08-07 and 2026-08-05 research-drop files.

## 2026-08-07 — Bard-primary trio roadmap

**Applied by:** Integration Agent, from `eql-bard-trio-roadmap.md` handed off directly in chat.

**New page — eql/trio-roadmap.html:**
- Hub page for the 7-trio no-overlap partition of all 16 classes into Bard-led trios: ranking logic (tank stance access, Divine invocation access, category-stacking bonuses), all 7 trio summaries (trio 1 marked done and linked to its existing deep-dive page; trios 2-7 marked planned with their full reasoning), the leftover-Rogue judgment call, and the summary table.
- Source explicitly flags this as original design synthesis / a prioritized build order, not sourced fact (no eqlwiki.com Bard-trio guide exists) — preserved that framing verbatim rather than presenting it as researched fact.
- **Site structure change:** repointed the homepage's trio card from linking directly to the Bard/Shadow Knight/Druid guide to linking to this new roadmap hub instead, since more trio guides are coming — avoids a card-per-trio homepage as the roadmap fills in. The hub itself links out to trio 1's guide.

Source: original design synthesis from confirmed Stances & Invocations mechanics, not a wiki transcription.
