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

## 2026-08-08 — Hunting grounds by class

**Applied by:** Integration Agent, from Bryan's direct chat request ("hunting grounds for each class... leveling path to maximize those efficiencies... Lower Guk is undead for Clerics as well as Befallen. The Hole has lots of summoned") — no research-drop file for this one, researched live via two delegated subagent passes against eqlwiki.com class/spell/zone pages.

**New page — eql/hunting-grounds.html:**
- Mechanic explainer for eqlwiki.com's Target Type field on damage spells; two confirmed restricted categories found: Undead and Construct/Elemental ("Summoned").
- Undead specialists with full spell chains: Necromancer (Ward Undead L6 → Expulse Undead L19 → Dismiss Undead L28 → Expel Undead L38 → Banish Undead L46), Paladin (Ward Undead L1 autogranted → Expulse Undead L30), Cleric (Ward Undead L4 → Expulse Undead L13), Shadow Knight (Ward Undead L18 → Expulse Undead L39). Zone table: Befallen, Estate of Unrest, Kithicor Forest, Lower Guk (ghoul side), Butcherblock Chessboard, The Hole (Undead Tower), Plane of Hate, Plane of Fear.
- Summoned specialists: Druid (Ward Summoned L2 → Expulse Summoned L13), Cleric (Ward Summoned L17 — only class confirmed with both categories), Magician (Ward Summoned L9), Ranger (Ward Summoned L16 → Dismiss Summoned L33). Zone table: The Hole (Golem Tower — directly confirms Bryan's own claim via a near-verbatim wiki quote), Solusek's Eye, Plane of Fear raid targets, Plane of Hate. Nagafen's Lair explicitly ruled out (insufficient type confirmation despite existing site flavor text).
- Explicit no-bonus list for the other 9 classes checked and cleared: Warrior, Rogue, Monk, Berserker, Beastlord, Shaman, Wizard, Enchanter, Bard — including notes on near-misses that don't count (Rogue's Assassinate is unimplemented, Wizard has no Giant/Dragon nuke, Shaman's Animal spells are non-damage).
- **Flagged, not presented as fact:** Necromancer's class-page claim of unique Animal/Plant-attacking spells — no matching spell found in its spell tables, likely flavor text. Mistmoore Castle's undead typing — strong vampire flavor but no confirmed Undead Creature Type tag found on NPC pages, unlike Hate/Fear which do carry that tagging.
- **Content gaps called out:** The Hole and Kithicor Forest are referenced with sourced level ranges/named mobs but are not yet in the Loot Codex's full 32-zone itemization — flagged for a future research pass.
- Linked from eql/index.html as a 6th card (`.card.hunt`, new `--violet` accent); 3-column grid wraps cleanly at 6 cards.

Source: eqlwiki.com spell pages (Ward Undead, Expulse Undead, Ward Summoned, Expulse Summoned, Dismiss Summoned, full class spell lists for all 16 classes) and zone pages (Estate of Unrest, Befallen, Lower Guk, Kithicor Woods, Butcherblock Mountains, The Hole, Solusek's Eye, Plane of Hate, Plane of Fear, Mistmoore Castle, Nagafen's Lair).

## 2026-08-11 — Spell lists for all 12 spellcasting classes

**Applied by:** Integration Agent, from Bryan's direct chat request ("research the latest information on spells. What spell lists do we have available now") — researched live via three delegated subagent passes against eqlwiki.com's per-class spell-table pages and main class pages (raw wikitext, to avoid fetch truncation on large tables).

**New page — eql/spell-lists.html:**
- Full level-by-level spell tables for all 12 spellcasting classes: Cleric, Paladin, Shaman, Druid, Necromancer, Magician, Wizard, Enchanter, Bard, Beastlord, Ranger, Shadow Knight — roughly 1,450 spells/songs itemized. Warrior, Rogue, Monk, and Berserker have no dedicated spell list on the wiki and are not included, matching the "no bonus" class list from the hunting-grounds page.
- Type-restricted damage spells (Undead / Construct-Elemental "Summoned") are tagged inline on each row and summarized per-class at the top of each section, cross-linked to the Hunting Grounds page.
- **Two corrections to the original hunting-grounds research pass, surfaced by this deeper spell-list research:** Druid's type-restricted line is Summoned-only, not both Undead and Summoned as originally implied — Cleric is the only class confirmed with both. Magician's Summoned line is a full 5-tier chain (Ward Summoned through Banish Summoned), not just the single base spell originally noted. Both corrections are called out explicitly on the new page; hunting-grounds.html itself was not rewritten this pass but should be read alongside this correction.
- **Known gap:** Enchanter is missing levels 46-50 — the source page exceeded fetch limits past level 45 on every attempt (current revision, two older revisions, and rendered HTML all truncated at the same point). Flagged on-page rather than guessed at.
- Condensed rather than itemized (for page usability): Cleric/Shaman/Druid's per-deity "Imbue [Gem]" spell families, Druid's ~75 zone-specific teleport spells, Wizard's ~65 travel spells (Gate/Portal/Translocate/Evacuate), and Enchanter's ~174 Level-1 cosmetic "Illusion: [race]" spells — all mechanically identical aside from destination/disguise.
- Data schema varies by source page: Cleric/Paladin/Shaman/Druid come from flat "All Spells" tables with no Skill or Location columns; the other 8 classes come from richer level-tiered tables that do carry Location (shown in Notes where not a plain Vendor purchase).
- Linked from eql/index.html as a 7th card (`.card.spelllists`, new `--teal` accent).

Source: eqlwiki.com — Cleric_Spells, Paladin_Spells, Shaman_Spells, Druid_Spells (flat tables), and the main class pages (action=raw wikitext) for Necromancer, Magician, Wizard, Enchanter, Bard, Beastlord, Ranger, Shadow Knight.

## 2026-09-11 — Dungeon crawl guide by level

**Applied by:** Integration Agent, from Bryan's direct chat request ("best dungeons to crawl by level range... XP, loot, named mobs, group size") — researched live by pulling eqlwiki.com's own "Per-Level Hunting Guide" page in full (rendered HTML truncated partway through, so the raw wikitext was fetched instead — both as a full page fetch and, for the two brackets still cut off, via the MediaWiki API's per-section raw endpoint to guarantee completeness).

**New page — eql/dungeon-crawl-guide.html:**
- All 316 hunting spots from eqlwiki.com's guide, transcribed across all 12 level brackets it defines (1-4 through 55-59) — zone, area/location, mob group, and the guide's own free-text notes (class-suitability tags, named-mob callouts, faction/quest hints, hazards).
- Preserved the source's own framing rather than imposing new structure: it's written as a solo-hunting guide by default ("Characters on this server generally perform like characters three or more levels higher..."), with group/CC needs surfaced only where the source calls them out in prose (e.g. "need some form of CC to break camp"), not as a fabricated column.
- The 55-59 bracket is confirmed as the de facto top of the guide — it folds in level-60 "buffer" camps (Plane of Fear, Skyshrine, Icewell Keep, Great Divide, etc.) rather than adding a separate 60+ section; no raid-tier bracket exists on this page.
- Linked from eql/index.html as an 8th card (`.card.dcg`, new `--rust` accent).

Source: eqlwiki.com/Per-Level_Hunting_Guide — Instructions, Legend, Hunting Spots 1-4 through 55-59, and Credits, pulled via full-page fetch plus targeted per-section raw wikitext fetches (sections 10 and 11, "Hunting Spots 30-34" and "35-39") to recover content lost to fetch-size truncation.

## 2026-09-11 — Dungeon Crawl required rares by zone (new 9/9/26 feature)

**Applied by:** Integration Agent, from Bryan's direct chat request ("this is a new feature as of 9/9/26 patch. We will need to focus on reddit and discord if possible. I would like to know a list of all the required rares for each zone") — researched via three parallel subagent passes covering 23 candidate zones (Antonica/Faydwer/Odus indoor dungeons + the 3 planes), since this feature was only 2 days old at research time and no wiki page yet compiles a per-zone rares list directly.

**New page — eql/dungeon-crawl-rares.html:**
- Confirmed the mechanic itself from eqlwiki.com/Dungeon_Crawl, which includes the game's own tooltip plus a verbatim Discord transcript from an EQL dev ("Secrets [EQL]") clarifying that rare-creature spawn *chance* is not increased by a Dungeon Crawl — these are each zone's pre-existing rare/named-flagged NPCs, now guaranteed to appear on the map. The dev also confirmed Plane of Sky now flags *all* mobs as rare (a change made this same patch) and Plane of Fear has zero labeled rares (crawl completion there runs on general-population kills alone).
- The one fully first-hand-documented run (a community blogger's Nagafen's Lair/Sol B crawl, 10 named required including one invisible mob) is quoted in full on the page as the reliability baseline — it's notable that 3 other well-known Sol B named mobs were *not* required, proving not every named NPC in a zone counts.
- For the other 21 zones covered, no source exposes the game's literal internal "rare" flag, so every entry is tagged with a confidence tier: wiki-confirmed (eqlwiki's Notable/Rare NPC field), explicit rare tag (a source flags it rare specifically, not just named), community-only (fan site/blog, not on eqlwiki's structured data), disputed (eqlwiki and EQLForge give conflicting rosters), or confirmed (dev/first-hand). ~169 creature entries total.
- Two zones (The Arena, Temple of Solusek Ro) are flagged as probable non-targets — no killable population was found for either — rather than guessing at a rares list for them.
- Per-zone caveats are called out inline where research surfaced them: Mistmoore Castle's day/night spawn cycle, Kedge Keep's water-breathing requirement, Highpass Hold's disputed indoor/outdoor classification, High Keep and Qeynos Aqueducts' conflicting source rosters, and several zones' see-invis/no-fixed-placeholder rares.
- Linked from eql/index.html as a 9th card (`.card.rares`, new `--crimson` accent). Cross-links to dungeon-crawl-guide.html with an explicit note that the two pages share a name coincidentally (that page predates this game feature and covers per-level hunting spots, unrelated to the Dungeon Crawl instance mechanic).
- **Standing caveat:** this is bleeding-edge content. Every list here should be treated as a best-available proxy pending in-game confirmation, not a guaranteed roster — re-verify anything time-sensitive before relying on it for a crawl.

Source: eqlwiki.com/Dungeon_Crawl (mechanic + Discord transcript), eqlwiki.com per-zone pages (raw wikitext, Notable/Rare NPC fields) for all 21 zones, cross-checked against eqlforge.com zone pages and chasingdings.com ("EverQuest Legends: The New Dungeon Crawl," 9/9/26, and "EverQuest Legends: Clearing Dungeons," 8/13/26).

## 2026-09-12 — Cazic Thule required rares, in-game verified

**Applied by:** Integration Agent, from Bryan's direct in-game verification ("I verified this myself") of the Cazic Thule Dungeon Crawl rares list, superseding the wiki/EQLForge-sourced proxy list from the 2026-09-11 pass.

**Updated — eql/dungeon-crawl-rares.html, Cazic Thule section:**
- Confirmed total is exactly 9 rares, up from the previous 5-entry proxy list.
- 8 of 9 confirmed by name with location and level: A Lizard Ritualist (Maze, 30), A Clay Golem (Maze, 25), Tae Ew Archon (Pyramid, 34), Cazic Cenobite (Avatar of Fear orb room), Tae Ew Diviner (Throne Room, 28), Tae Ew Templar (Throne Room, 28), Steel Golem (Alligator Pit, 37), Stone Golem (Off Throne Room, 29).
- 9th rare not identified — Bryan confirmed it exists (to reach the total of 9) but couldn't recall the name. Explicitly confirmed **not** Radiant.
- Radiant and Avatar of Fear, both carried over from the original wiki-sourced list, are now confirmed **excluded** from the required set — first real case in this dataset of the "not every named NPC counts" pattern (matching the Sol B precedent) being independently confirmed by a second source.
- All 8 named entries upgraded to the "Confirmed (dev/first-hand)" tier; the missing 9th is tagged "Disputed" pending identification.

Source: Bryan's own in-game Dungeon Crawl completion of Cazic Thule, 2026-09-12.

## 2026-09-12 — Cazic Thule correction: Avatar of Fear is required

**Applied by:** Integration Agent, from Bryan's direct correction ("Avatar of Fear is required") to the same-day Cazic Thule update, which had wrongly carried Avatar of Fear over as a confirmed exclusion.

**Updated — eql/dungeon-crawl-rares.html, Cazic Thule section:** Avatar of Fear now fills the 9th (previously unidentified) rare slot, tagged "Confirmed (dev/first-hand)." Radiant remains confirmed excluded — that part of the earlier correction stands. The zone's confirmed 9-rare roster is now complete: A Lizard Ritualist, A Clay Golem, Tae Ew Archon, Cazic Cenobite, Tae Ew Diviner, Tae Ew Templar, Steel Golem, Stone Golem, Avatar of Fear.

Source: Bryan's own in-game verification, 2026-09-12.

## 2026-09-12 — Cazic Thule 9th rare identified via combat log

**Applied by:** Integration Agent, cross-referencing Bryan's connected EverQuest Legends install (D:\Everquest\Logs\eqlog_Catseye_qeynos.txt) after his verbal correction that Avatar of Fear is required. The full combat log for his Fri Sep 11 08:11–09:13 Cazic Thule Dungeon Crawl shows exactly 9 distinct named/rare "You have slain" lines, matching his reported total precisely: Tae Ew Archon, Cazic Cenobite, Tae Ew Templar, Tae Ew Diviner, a lizard ritualist, a clay golem, a steel golem, a stone golem, and Avatar of Fear pet.

**Correction — eql/dungeon-crawl-rares.html, Cazic Thule section:** the 9th rare is **Avatar of Fear pet** (a pet/add that spawns during the Avatar of Fear encounter), not the Avatar of Fear boss itself as the previous same-day update stated. This is now log-verified rather than recalled from memory — the highest-confidence source available for this zone.

Source: Bryan's own EverQuest Legends combat log, connected folder D:\Everquest\Logs, entries timestamped 2026-09-11 08:11:59–09:13:23.

## 2026-09-12 — Lower Guk required rares, log-verified

**Applied by:** Integration Agent, from Bryan's own Lower Guk Dungeon Crawl tally ("Total Rares: 25," 24 listed, "I'm missing 1 kill") cross-referenced against his connected EverQuest Legends combat log (D:\Everquest\Logs\eqlog_Catseye_qeynos.txt), covering his Sat Sep 12, 00:30–02:45 run.

**Updated — eql/dungeon-crawl-rares.html, Lower Guk section:** replaced the previous 13-entry wiki/EQLForge-sourced proxy list (several rows were grouped slashes, e.g. "A Ghoul Cavalier / Executioner / Savant...") with the full 25-entry log-verified roster, each tagged with Dead Side/Live Side location. All 24 of Bryan's listed rares check out in the log — several were credited to his pet ("X has been slain by Catseye`s warder") rather than to him directly, likely why they were easy to miss from memory. One naming correction: the Ghoul Lord's actual in-game name is **Hoptor Thaggelum**, not "Hopptor" — he has his own pet (Hoptor Thaggelum pet) that also dies in the fight.

**25th rare — narrowed, not yet confirmed:** cross-checking every "slain" line in the run for singleton kills (died exactly once, vs. population trash which died many times) surfaced exactly two candidates not on Bryan's list: a froglok nok shaman and a froglok yun shaman (both Live Side). Everything else that died once is already one of the 24; everything that died multiple times (wan/zol/dar/vis ghoul knights, ghoul wizards of various castes, greater minotaurs, greater ice bones, basalt gargoyle, vampire bat) is population trash, not a rare. Flagged "Disputed" pending Bryan's confirmation of which one.

**Note:** Slaythe the Slayer and A Basalt Gargoyle, both carried over from the original wiki-sourced list, did NOT appear as singleton/rare-pattern kills in this run's log (gargoyle died 3 times = trash; Slaythe didn't appear at all) — removed from the required-rares table. They may still exist as zone NPCs, just not part of this crawl's required set, matching the Cazic Thule precedent (not every named NPC counts).

Source: Bryan's own EverQuest Legends combat log, connected folder D:\Everquest\Logs, entries timestamped 2026-09-12 00:30:xx–02:45:45, cross-referenced against Bryan's manually reported 24-item list.

## 2026-09-14 — The Warrens required rares, log-verified and confirmed

**Applied by:** Integration Agent, from Bryan's own Warrens Dungeon Crawl tally cross-referenced against his connected EverQuest Legends combat log (D:\Everquest\Logs\eqlog_Catseye_qeynos.txt), covering his Mon Sep 14, 08:48–11:13 run — then reconciled against his final confirmed 18-item list.

**Updated — eql/dungeon-crawl-rares.html, The Warrens section:** replaced the previous 9-entry wiki-sourced proxy list (several grouped slash-rows) with the full 18-entry confirmed roster, each tagged with level where Bryan supplied it. Log analysis of the run initially surfaced 21 candidate named kills; Bryan's own review of his tracker pared this to the correct 18. Four names killed during the run were confirmed **not** part of the required set: A Kobold Master Blacksmith, Koajin, Kujanko, and Owakanji — matching the established pattern that not every named/proper-noun NPC a player kills counts toward a zone's Dungeon Crawl requirement (see Cazic Thule's Radiant exclusion and Nagafen's Lair's King Tranix/Warlord Skarlon/Magus Rokyl exclusions).

**Notable log detail:** The Mighty Bear Paw (confirmed required, level 24) was mid-fight in the log — a long, dangerous encounter (healing pet, Chaos Flux nuke, killed Bryan twice) — right up to the exact second the crawl registered complete, with no explicit "has been slain" line captured in the window. Included per Bryan's confirmation despite the ambiguous log ending.

Source: Bryan's own EverQuest Legends combat log, connected folder D:\Everquest\Logs, entries timestamped 2026-09-14 08:48–11:13, reconciled against Bryan's manually reported and corrected 18-item list.

## 2026-09-15 — Plane of Hate/Fear armor sets, converted to per-class table

**Applied by:** Integration Agent, from Bryan's request to identify which Plane of Hate/Fear armor set belongs to each class, then turn the answer into a proper table on the site.

**Updated — eql/planes-of-power.html, Loot Groups sections (Hate and Fear):** the existing prose bullet lists (from the original research pass) already had this data but buried in parenthetical class-code shorthand — converted both into a shared 18-row table (16 classes + the two class-unrestricted bonus sets, Lustrous Russet and Midnight Clad Armor) with a Group 1/Group 2 pool column. Confirmed via the existing research that Hate and Fear drop identical set names/class assignments — the Fear section now states this explicitly instead of repeating the full list, with its own table for scannability.

No new research was needed — this was a presentation upgrade of already-sourced data (originally from eqlwiki.com per the 2026-08 planes-of-power.html build).

Source: eql/planes-of-power.html's existing Loot Groups content (unchanged data, restructured presentation).
