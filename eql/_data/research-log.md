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
