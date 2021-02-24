# About this config
* Requires BH>=1.9.8 (planqi branch)
* Items are grouped into tiers based on relative worth. Worth is loosely defined as some combination of usefulness and rarity.
* Consistent colors are used to indicate the item tiers. The map box and item name indicator (leading 0) colors always match.
  - Tier1 (Orange): The good stuff. Sur, ber, jah, griff's, etc.
  - Tier2 (Purple): Vexes, ohms, arachs, high end socketables, etc.
  - Tier3 (Red): Tal armor, shako, etc.
  - Tier4 (Gold): Occy, titan's, vmagi, etc.
  - Tier5 (Green): Magefist, TO gloves, Tal belt, etc.
* Many useful shoppables are highlighted, including ladder reset stuff.
* Tries to ping every usable unique and set item. Useless ones are not hidden but will not ping.
* Tries to ping every useful socketable, including plague bases.
* Useful charged items are highlighted: life tap wands, lower resist wands, teleport staves
* The item filter works on an item by item basis. Only the junkiest stuff is hidden. Nothing is hidden with clvl<40. There is little risk that useful things are blocked by this filter.
* Does not attempt to judge the value of identified rare/crafted/magic items. Does ping unidentified rare/magic items worth IDing.
* Shows affix level on magic, rare, and crafted items when it is different from ilvl. The format is ilvl/alvl.

# M81's Releases
See the [ Old releases](https://github.com/youbetterdont/bhconfig/releases) page for the latest version and change log.


# LeBron's BH.cfg Compared to m81's latest config v2.5.9
* Differentiated a bit more between filter level 1 and 2 on some items, mostly to add a gap for the first week or two after a ladder reset until endgame filter levels 2 and aggressive.
* Added classic shopping section that's commented out (uncomment if playing classic)
* Added classic stuff section that's commented out (uncomment if playing classic)

* Gems:

  - Flawless topaz and rubys notify if filtlvl 0
  - Flawless topaz and rubys notify if filtlvl 1 with tier 6 only
  - Flawless diamonds notify if filvlvl is 0 or 1 and char level is under 40 and tier=6
  - chipped, flawed, and regular topaz's, rubys, saphires notify if filtlvl 0 and char lvl under 20
  - flawed+ diamonds notify if filtlvl 0 and char lvl under 26
  - chipped gems for repairing show up as a small gray dot on map if filtlvl is 0 or 1 and tier =4

* Runes:

  - rals and hels lines are tier 5
  - spirit rune sets get small green dots with filtlvl 0 and 1 and tier 5
  - insight runes get small pink dots with filtlvl 0 and 1 and tier 5
  - orts for reparing get small gray dot if filtlvl 0 or 1 and tier 4
  - Ko and fal get pinged if filtlvl 0 or 1 and tier 5
  - Ko and fal get dots if filtlvl over 2 and tier 5
  - Tir to fal get pinged if fitlvl 0 and tier 5
  - tir to fal get pinged if filtlvl 1 and tier 6
  - el and eld runes for upping/botd get pinged if filtlvl 0 or 1 and tier 6

* Tier 6 (ladder reset stuff)
  -demonhide and sharkskin belts ping on early levels

* Shoppables colored (and get pinged if dropped early in leveling process with tier 6) all these are shoppable from acts 1 and 2 normal:
  - +2-3 charged bolt staff
  - fcr wands, staves, and scepters
  - 3os large and kite shields
  - frw boots
  - FHR belts, armors, and shields get orange names
  - 2 socket helms for lore/runes
  - 2 socket armors for stealth
  - 2 socket small shields
  - 3 socket armors 
  - 3 socket spetum 
  - 3 socket flails 
  - 2 socket staves with 3 warmth
  - 2 socket staves with + to enchant
  - 0 or 4 socket staff with enchant (memory)
  - 3 prayer white or 3 socket grand scepter (plague) -slash specific

* Uniques:
- Tier 5
  - Hellmouth (war Gauntlets)
  - Spellsteel (Bearded Axe)
  - M'avina's Tenet (Belt)
  - Natalya's Soul (Boots)
  - Medusa's Gaze (Shield)
  - Cleglaw's Pincers (Chain Gloves / Bracers)
  - Maelstrom (Yew Wand) only if filter = 0
  - made herb t3
  - made token tier 3

* Socketables:
- Tier 3
  - 3 chant, 1+ FM orb capable of 3os (plague) -Slash Specific
  - 3 Energy shield ES orb capable of 3os (plague) -Slash Specific
  - 0os ETH monarch ebuggable (spirit)
- Tier 4
  - changed map dots from gold to white dot with gold border for all Tier 4 socketables
- Tier 5
  - 4os ETH monarch (spirit)
  - 3os dusk shrouds
  - ping only top 10% 3os dusk shroud, wyrmhide, scarab husk, wire fleece, great hauberk. Previously it would ping all 0/3/4os
  - ping only top 20% 3os Archon Plates. Previously it would ping all 0/3/4os
  - 6os phase blade (Gold find / Last wish / 6 ist)
  - 2 chant orb capable of 3os (plague) -Slash Specific
  - 1 chant 1 ES orb capable of 3os (plague) -Slash Specific
  - 1 energy shield ES orb capable of 3os (plague)
  - 3os Archon Plate any defense eth/non eth
  - 0os or 3os Archon Plate (top 20%)
  - 3os Archon Plate superior any ED
  - inferior archon plates able to get 3os with cube recipe
- Tier 6
  - added cap of char level 60 to pings for 0os polearms that get 4 sockets from Larzuk and removed CV's (too high str req)
  - 3os masks (mask only helms for low str req) 
  - 3os helms (others for merc/ higher str req excluding spired helms and coronas)
  - 3os eth, reasonable req 1h sword/axe (cmoon) (Changed from tier 4 to tier 6)
  - 0/3os/4os Dusk shroud, wyrmhide, scarab husk, wire fleece, great hauberk (top 10%) moved to tier 6 (previously tier 4)
  - 0/3os/4os archon plates (top 20%) moved to tier 6 (previously tier 4)
  - 3os gothic and ancient armor with ED (enigma) moved to tier 6 (previously tier 4)
  - 0/6os eth archon staff (wolf botd) moved to tier 6 (previously tier 4)
  - 0/6os eth glorious axe (wolf botd) moved to tier 6 (previously tier 4)
  - 0/6os eth thunder maul (wolf botd) moved to tier 6 (previously tier 4)
  - Eth Ettin Axe 0/5os with ED (death) moved to tier 6 (previously tier 4)
  - 4os phase blade (Passion) moved to tier 6 (previously tier 4)
  - imbuable diadems moved to tier 6 (previously tier 5)

* Magic items:
- Tier 4
  - Grand charms show blue border with gray dot
  - Made jewels a seperate lines
  - small charms show blue border with green dot and orange pixel
- Tier 6
  - eth magic circlets added
  - Sharkskin and vampirefang belts for crafting added 
  - large charms added ping only if filtlvl 0 or 1 with tier 6
- Magic Amulets
  - magic amulets show green dot if craft level = 90 or more
  - magic amulets Ping if filter level 0, just map box if filter level 0 and 1 and tier 5
  - magic amulets orange dot and ping for magic amulets ilvl 88+ for filter levels 0 and 1 and Tier 5
  - magic amulets orange dot and map box but no ping magic amulets ilvl 88+ for filterl level 2 and tier 5

* Rare items:
- Tier 4
  - rare amulets ping only if filter level 0 or 1. yellow border with black dot on map
  - rare amulets filter level 2+ show map box but no ping tier 5. yellow border with black dot on map
- Tier 5
  - rare jewels ping only if filter level 0 or 1. yellow border with black dot on map
  - rare jewels filter level 2+ show map box but no ping tier 5. yellow border with black dot on map
  - rare boots ping only if filter level 0 or 1. yellow border with black dot on map
  - rare boots filter level 2+ show map box but no ping tier 5. yellow border with black dot on map
  - rare gloves ping only if filter level 0 or 1. yellow border with black dot on map
  - rare gloves filter level 2+ show map box but no ping tier 5. yellow border with black dot on map
- Tier 6
  - added rare belts under 60str ping only if filter level 0 or 1. yellow border with black dot on map
  - added rare belts under 60str filter level 2+ show map box but no ping tier 6. yellow border with black dot on map

* Other:
  - Show price of items if clvl is under 35 and filter level is 0
  - Items worth good gold will have $ and prices in front
  - Progressive potions display based on clvl to show low HP, Mana, stamina, antidote, thawing, and strangle potions on all filtlvls
  - Progressive trailing gold prices when filtlvl under 2 for items. (e.g. 25k in norm, 35k in hell) Might be slightly off in normal as it's clvl based instead.
  - added display weapon range and speed line (uncommented to use)
  - added display ilvl line (uncomment to use)
  - Rejuv and full rejuves changed to R1 and R2 respectively
  - Hide gold piles under 100 if char level is over level 2.
  - Hide gold piles under 1000 if char level is over 19.
  - Default hide piles over 3000 if filter level is over 0.
  - unhide greater mana and health potions if filter level over 0 (M4 and HP4)
  - fixed description for greater and super mana and health potions
  - added item description for  2os exceptional Spears or Polearms - Strength runeword

# LeBron's BH_Settings.cfg Compared to m81's v1.4
* show automap on join option
* Skip NPC quest messages option
* Show settings option
* Added screeninfo congif for xp info
* Rejuv button
* always view loot option
* run tracker info
* Mustache template for stash export
