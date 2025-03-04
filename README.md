# About this config

These files were designed for SlashDiablo but can be used elsewhere since Slash is vanilla D2 with very few changes. 
These are close to M81's (SlashDiablo default) BH maphack config tier system with quite a bit of changes to add QoL for low levels + some endgame things. Lots of changes are all logged in the link below. More user friendly and noob friendly with identified tiers for all types of items and labels for easy editing. The settings file also utilizes the beta features added by DannyIsGreat like showing all items on the ground without holding a button and tracking your runs for you.
This version makes it super easy to add items for your holy grail needs as well. It can also be used in classic D2 mode with it's own separate tiers and filters!

# INSTALLATION INSTRUCTIONS
* Close all Diablo 2
* Backup your `BH.cfg` file in the diablo 2 folder if you care for your old config
* In SlashDiablo launcher set Maphack Version to None and Override to  ON
* Patch/update with Launcher
* Download `BH.cfg`, `buffs.mpq`, `BH_settings.cfg` and `BH.dll` from the releases page [here](https://github.com/BeLikeLeBron/bhconfig/releases/latest) and Put them into your Diablo 2 Slash Diablo folder. `buffs.mpq` is required to show the current active buffs on the screen (All the mpq contains is a dc6 file with the buff icons scaled down).
* In game you can toggle permanently show items on ground (press L 1 time to toggle)
* Run tracker - Track xp and drops for your character. File saved in ./data/%CHARNAME%.csv, a folder called data in your slashDiablo directory 
* You can now also use the run tracker infographic with these run log files https://redd.it/khhgha
* Recommended filter level 1 and ping level 5 or 6, but use whatever you want depending on what items you want notifications for (pings) and what you want to see on the ground (filter)!
* User guide here https://github.com/BeLikeLeBron/bhconfig/wiki/User-Guide
* Enjoy 

- Requires Danny's BETA BH>=1.9.9 for BH_Setting.cfg.
- BH.cfg and BH-classic.cfg Require BH>=1.9.9 (Planqi 1.9.9 or Danny’s beta)
- dschu012's (Danny's) beta BH.dll attached below. USE THIS ONE. More info on it [here](https://github.com/BeLikeLeBron/bhconfig#dschu012s-dannys-bhcfg-beta-features)
     - [BH.cfg Changes logged here](https://github.com/BeLikeLeBron/bhconfig#lebrons-bhcfg-compared-to-m81s-last-config-v259-slashdiablo-default)
     - [BH-classic.cfg features logged here](https://github.com/BeLikeLeBron/bhconfig#lebrons-bh-classiccfg)
     - [BH settings changes logged here](https://github.com/BeLikeLeBron/bhconfig/blob/master/README.md#lebrons-bh_settingscfg-compared-to-m81s-v14)
     - Default Planqi BH.dll 1.9.9 (official release) [here for reference](https://github.com/planqi/slashdiablo-maphack/releases)

# Adding Holy Grail items to config
* Our configs already include many of the holy grail items you're looking for, but if you want to add All missing grailers you have a couple of options:
* Automated method:
     * -1. Download and install the [slashDiablo chrome extensions](https://chrome.google.com/webstore/detail/slash-diablo-tools/hfbigecinjgkbmdldhgogmdjfblpkagp) via google chrome, if you have it installed already, make sure it's updated
     * -2. Restart the browser, then navigate to your grail.slashdiablo.net account, There will be a button on the top right for "BH Filter Missing Items". click it. It will copy all lines for your missing items list for that account.
     * -3. Make sure to turn on maphack override option in SlashDiablo launcher before editing your bh.cfg file. Close D2 and any errors. Then in your BH.cfg file in your SlashDiablo/d2 folder under the section labeled "ADD HOLY GRAIL ITEMS HERE" paste them and save. If you don't see that line, you can add these items directly under the "UNIQUES AND SETS" part of your BH.cfg config and it should work perfectly. You can do this periodically and replace these lines in your config as you find items instead of refreshing it manually. Save it. You're done!
* If you want to do this manually or want to add something specific:
     *  Go [here](https://github.com/BeLikeLeBron/bhconfig/blob/master/Holy_Grail_All_Uniques_and_Sets.txt) for a list of all uniques and set lines that are ready to be used. All uniques are Tier 4 items there, All sets are Tier 5 items. Feel free to change them as you wish. Simply copy the lines you want from that link then follow step 3 above. 
     *  BE WARNED: your ping level must match the lines TIER number in the in-game BH settings to notify you of the drop
     *  %TIER-X% REQUIRES BH 1.9.9 to work. If you don't want to use on 1.9.9, simply remove %TIER-x% from all the lines.



# Config basics
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
* Config [User guide](https://github.com/BeLikeLeBron/bhconfig/wiki/User-Guide)
* how to Edit the config [guide](https://github.com/BeLikeLeBron/bhconfig/wiki/How-to-edit-the-config)
* Color palette and item information can be found either in [here](https://github.com/planqi/slashdiablo-maphack/wiki) or [here](https://github.com/underbent/slashdiablo-maphack/wiki)

# M81's Releases
This is for the SlashDiablo default reference files. See the [Old releases](https://github.com/youbetterdont/bhconfig/releases) page for the change logs.


# BH.DLL 1.9.10 features
* CURRENTLY IN BETA!
* Comes with everything on Planqi's 1.9.9(default with SlashDiablo launcher) but with some new features on top such as:
* Added show Buff/debuff system so you can view the current active buffs on your character (such as BO and Auras) (credit Arolds) 
* Updated Dec 12 2020 (added player count column, session counter)
* Show Automap on Join
* permanently show items on ground (press L 1 time to toggle)
* enhancements to see xp stats of pervious run on top right of screen info
* Auto skip npc quest messages
* Hotkey to use rejuv potions from inventory
* Item mover features fixed with plugy
* Classic filter option for CLASSIC lines (and !CLASSIC for expansion only lines)
* Area level shown in top right of hud
* Configurable stat range colors (default dark green)
* Custom colors for monster enchantments and auras configurable in Bh_Settings.cfg
* Run tracker - Track xp and drops for your character. File saved in `./data/%CHARNAME%.csv`, a folder called `data` in your SlashDiablo directory 
* Note: in BH_settings.cfg `Run Details Ping Level` is the ping level of items you want to record (default ping level 4). You can add `%notrack%`  in your config if you want to disable tracking of certain  items like charms/gems.
* More details here about this BH version can be found in dschu012's pull requests [here](https://github.com/planqi/slashdiablo-maphack/pulls)


# LeBron's BH_Settings.cfg Compared to m81's v1.4
* show automap on join option
* Skip NPC quest messages option
* Show settings option
* Added screeninfo congif for xp info
* Rejuv button
* always view loot option
* Highlight Chaos Seal bosses/ubers on minimap (purple color)
* Run tracker info
* Tp button 5 (customizable)
* Custom monster enchantments (conviction bosses highlighted yellow)
* Area levels shown
* more descriptions and instructions
* Mustache template for stash export

# Classic Features
* has many nice features mentioned above and below that use the filtlvl and ping lvl's just like the expansion one, but dedicated to classic items only.
* It's now combined into the BH.cfg on this page.
* Note: BH-Classic.cfg will be the final version of this classic config as it's now all combined into the bh.cfg file for future versions. Keeping this BH-Classic version here because it is backwards compatible with older bh.dll files pre 1.9.10. To be used only in classic mode of Diablo 2. Rename to BH.cfg before use. more detailed instructions in the classic config file.

# LeBron's BH.cfg Compared to m81's last config v2.5.9 (slashdiablo default)
* Differentiated a bit more between filter level 1 and 2 on some items, mostly to add a gap for the first week or two after a ladder reset until endgame filter levels 2 and 3.
* Added pings for some missing items
* Added tiers for identified magic items
* Added ability to easily expand with holy grail items to utilize the new SlashDiablo Holy Grail system with the slash chrome extension or [all uniques and sets listed here](https://github.com/BeLikeLeBron/bhconfig/blob/master/Holy_Grail_All_Uniques_and_Sets.txt)
* Added more info and links to help players customize and achieve what they want
* Most old lines maintanined if users feel like using the older ones instead.
* Order tiers so it's more legible separated sets/uniques and armors/weapons on white/magics/rares
* Tiers for identified Items (uniques/sets/magics/rares/crafts)
* classic compatible lines + customization features/tiers/descriptions
* better descriptions, logging, and easy instructions added.
* Many other features not logged here, but logged in the actual Bh.cfg file.

* Gems:

  - Flawless topaz and rubys notify if filtlvl 0 and 1 with tier 6 only
  - Flawless diamonds notify if filvlvl is 0 or 1 and char level is under 40 and tier=6
  - chipped, flawed, and regular topaz's, ruby's, sapphires notify if filtlvl 0 and char lvl under 20
  - flawed+ diamonds notify if filtlvl 0 and char lvl under 26
  - chipped gems for repairing show up as a small gray dot on map if filtlvl is 0 or 1 and tier =4

* Runes:

  - Ko and fal get pinged if filtlvl 0 or 1 and tier 5
  - Ko and fal get dots if filtlvl over 2 and tier 5
  - added sol lines to behave like rals for ring crafting (uncomment // to use)
  - spirit rune sets get small green dots with filtlvl 0 and 1 and tier 6
  - insight runes get small red dots with filtlvl 0 and 1 and tier 6
  - orts for repairing get small gray dot if filtlvl 0 or 1 and tier 4
  - low runes get pinged if fitlvl 0 and tier 6
  - Map lines added for tier 1 and 2 runes
  - added description for gul and Herb for dclone spawn instructions (slash specific)

* Tier 6 (ladder reset stuff)
  - demonhide and sharkskin belts ping on early levels
  - crafted caster belt bases ping up to level 80 for filtlvl 0 and 1

* Shoppables colored (and get pinged if dropped early in leveling process with tier 6) all these are shoppable from acts 1 and 2 normal:
  - Fixed color on all shoppable items so it's colorblind friendly with stars
  - +2-3 charged bolt staff
  - fcr wands, staves, and scepters
  - 3os large and kite shields
  - frw boots
  - FHR belts, armors, and shields get orange names
  - 2 socket helms for lore/runes
  - 2 socket armors for stealth
  - 2 socket small shields
  - 3 socket armors 
  - 3 socket septum 
  - 3 socket flails 
  - 2 socket staves with 3 warmth
  - 2 socket staves with + to enchant
  - 0 or 4 socket staff with enchant (memory)
  - 3 prayer white or 3 socket grand scepter (plague) -slash specific

* Metadata:
  - added weapon range and speed lines for all items (uncomment // to use)
  - added ilvl and price display lines for all items (uncomment // to use)

* Added holy grail section
  - Easily add uniques and sets using the provided area and instructions. Use either the [SlashDiablo chrome extensions](https://chrome.google.com/webstore/detail/slash-diablo-tools/hfbigecinjgkbmdldhgogmdjfblpkagp) or the list [here](https://github.com/BeLikeLeBron/bhconfig/blob/master/Holy_Grail_All_Uniques_and_Sets.txt) to add items into this section of the config
  - added ping all uniques/set optional lines in this section that are off by default (uncomment // to use) 
 
* Uniques:
- Tier 1
  - Added Map lines for tier 1 and 2 uniques
- Tier 2
  - Added fireball and frost nova Ormus's here along with the other good Ormus's
- Tier 3
  - added Herb for dclone spawn (slash specific)
  - Added token of absolution
- Tier 5
  - Fixed suicide branch item code
  - Hellmouth (war Gauntlets)
  - Spellsteel (Bearded Axe)
  - M'avina's Tenet (Belt)
  - Natalya's Soul (Boots)
  - Medusa's Gaze (Shield)
  - Cleglaw's Pincers (Chain Gloves / Bracers) only if filter = 0
  - Maelstrom (Yew Wand) only if filter = 0
  - Eth Gimmershred (flying axe)
- Tier 6
  - Gerke's Sanctuary (shield)
  - Angelic's set rings only if filter = 0
  - Death's Hand (Leather Gloves) only if filter = 0
  - Death's Guard (Sash) only if filter = 0
  - Hsarus' Iron Stay (Belt) only if filter = 0
  - Hsarus' Iron Heel (Chain Boots) only if filter = 0
  - The Ward (Gothic Shield) only if filter = 0
  - Wall of the Eyeless (Bone Shield) only if filter = 0
- Identified unique and set tiers added
- Classic uniques/sets added for use with classic automatically

* Socketables:
- Tier 3
  - 3 chant, 1+ FM orb capable of 3os (plague) -Slash Specific
  - made 15ed Mage plates t3 for enigma bases (previously t4)
  - added lines for assassin weapon bases with 3LS + 1-3 DS (plague) -Slash Specific
- Tier 4
  - changed map dots from gold to white dot with gold border for all Tier 4 socketables so it's less confusing with uniques
  - top 3 socket elite armors
  - 0os ETH monarch ebuggable (spirit)
  - 3 chant orb capable of 3os (plague) -Slash Specific
  - 3 Energy shield ES orb capable of 3os (plague) -Slash Specific (uncomment // to use)
 
- Tier 5
  - 4os ETH monarch (spirit)
  - 3os gothic and ancient armors with ED moved to tier 5 (previously tier 4)
  - 6os phase blade (Gold find / Last wish / 6 ist)
  - 2 chant orb capable of 3os (plague) -Slash Specific
  - 1 chant 1 ES orb capable of 3os (plague) -Slash Specific (uncomment // to use)
  - 1 energy shield ES orb capable of 3os (plague) (uncomment // to use)
  - 0os Archon Plate (top 20%) non superior (uncomment // to use)
  - inferior archon plates able to get 3os with cube recipe (uncomment // to use)
- Tier 6
  - added cap of char level 60 to pings for 0os polearms that get 4 sockets from Larzuk and removed CV's (too high str req)
  - Added 2 lines for 0os CV's that get 4 sockets from Larzuk, no notification by default, if you want notification uncomment // to use
  - 3os masks (mask only helms for low str req) 
  - 3os helms (others for merc/ higher str req excluding spired helms and coronas)
  - 3os eth, reasonable req 1h sword/axe (cmoon) (Changed from tier 4 to tier 6)
  - crystal swords with 3 sockets for plague/cmoon/lawbringer
  - 0/4os Dusk shroud, wyrmhide, scarab husk, wire fleece, great hauberk (top 10%) moved to tier 6 (previously tier 4)
  - 0/4os archon plates (top 20%) moved to tier 6 (previously tier 4)
  - 0/6os eth archon staff (wolf botd) moved to tier 6 (previously tier 4)
  - 0/6os eth glorious axe (wolf botd) moved to tier 6 (previously tier 4)
  - 0/6os eth thunder maul (wolf botd) moved to tier 6 (previously tier 4)
  - Eth Ettin Axe 0/5os with ED (death) moved to tier 6 (previously tier 4)
  - 4os phase blade (Passion) moved to tier 6 (previously tier 4)
  - 2os/3os eth elite armors added for merc on filter lvel 0 and 1 only
  - 0/4/5os elite polearms for insight/obedience added (non cv) on filter level 0 and 1 only
  - 2os exceptional spears/polearms for strength runeword when char lvl is under 60
  - masks that get 3 sockets from Larzuk when char lvl is under 45
  - 3os mage plates added
  - 3os elite armor bases with lower defenses added here
  - imbuable diadems moved to tier 6 (previously tier 5)

* Misc:
- Essences and uber organs added
- whitelisted some 3 socket armor bases
- whitelisted 6 socket crystal swords

* Magic items: 
- Made boxes on map more visibly appealing (you can tell what dropped by just looking at the different box style)
- Tier 3
  - Grand charms from Baal, Diablo, Nihlathak for potential 45 lifers
- Tier 4
  - Grand charms show blue border with gray dot
  - Made jewels a separate lines
  - small charms show blue border with green dot and orange pixel
- Tier 6
  - eth magic circlets added
  - Sharkskin and vampirefang belts for crafting added when filter lvl 0 or 1
  - large charms added ping only if filtlvl 0 or 1 with tier 6
- Magic Amulets
  - magic amulets show green dot if craft level = 90 or more
  - magic amulets Ping if filter level 0 and tier 5
  - magic amulets ping if filter level 1 and tier 6
  - magic amulets ilvl 88+ ping if filter level 1 and tier 5
- Classic Magic tiers added for use with classic automatically
- Identified Magic tiers added

* Rare items:
- Made boxes on map more visibly appealing (you can tell what dropped by just looking at the different box style)
- Tier 4
  - rare amulets are still t4 except for potential +2 class skill amulets from Baal, Diablo, and Nihlathak (those are t3).
- Tier 5
  - rare jewels are now t5 (previously tier 4)
  - rare boots (not Myrmidon - too high str req) ping t5
  - rare gloves (not Ogre Gauntlets - too high str req) ping t5
  - Added a rare weapons and eth weapons of interest section (remove // to use these lines)
- Tier 6
  - added rare belts under 150 str req with 4 box rows ping t6.
- Whitelist
  - Rare Ogre Gauntlets
  - Rare Myrmidon Boots
  - Rare Troll belts and Colossus Girdle
- Classic rare tiers added for use with classic automatically
- Identified Rare tiers added

* Other:
  - Identified Crafted tiers added
  - Classic custom lines throughout the config and filtering + descriptions added for classic d2 mode.
  - Rejuves are +R1 and +R2+. made the white dot purple. 
  - Greater potions are not hidden on filter level 1, hidden on filter level 2+ automatically.
  - Items worth good gold will have $ and prices in front
  - Progressive potions display based on clvl to show low HP, Mana, stamina, antidote, thawing, and strangle potions on all filtlvls
  - Progressive trailing gold prices on items when filtlvl under 2 for items. (e.g. 25k in norm, 35k in hell) Might be slightly off in normal as it's clvl based instead.
  - show actual value of items if level is under 15 and item is worth 1k+ gold (400+ in very early levels) 
  - Hide gold piles under 100 if char level is over level 3
  - Hide gold piles under 1000 if char level is over 19.
  - Default hide piles over 3000 if filter level is over 0.
  - unhide greater mana and health potions if filter level over 0 (M4 and HP4)
  - fixed description for greater and super mana and health potions
  - added item description for  2os exceptional Spears or Polearms - Strength runeword
  - added tp scrolls, id scrolls, and keys to be hidden if filtlvl=3 (remove // to use these lines)
  - Certain useless Rare weapons hidden on filtlvl=2 (non eth only)
  - potion filter sectioned and clarified for customizability
