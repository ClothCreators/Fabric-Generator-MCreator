# Changelogs:
## 1.1
### Snapshot 2
* Updated Fabric API to 0.34.6
* Added a complete support for the game rule mod element
* Added new world procedure blocks: get logic game rule, get number game rule, set logic game rule and set number game rule  
* [Bugfix #110] GROUND and PLANT step sounds had the wrong sound.

### Snapshot 1
* [#83] Added support for custom living entities
  Note: Flying entities are not 100% implemented. Entity inventory and Ranged attacks are not implemented.
* Added minimum and maximal enchantment level parameters
* Added Enable melee damage checkbox for custom items
* [Bugfix #102] Some block triggers caused build errors
* [Bugfix #105] Blocks mined with a tool using a lower harvest level dropped. 
* [Bugfix] Some sound mappings did not work properly

## 1.0.2
* [Bugfix #99] Repair items could not use custom tools
* [Bugfix #101] Select a map color on custom blocks caused a build error
* [Bugfix #102] Some block triggers caused build errors
* [Bugfix #102] Several world procedure blocks caused a build error  
* [Bugfix] Some Material mappings were wrong  
* [Bugfix] Custom plants prevented the workspace compilation

## 1.0.1
* Updated to MCreator EAP 2021.12313
* Updated Fabric API to 0.32.5
* Updated the command mod element to support new features
* Updated the block and plant mod elements to support the new bounding box editor
* [#72] Bounding boxes now properly rotate
* Added grass model for blocks
* Added new block/plant properties: Step sound, speed and jump factors
* [Bugfix] Custom blocks did not compile due to the new bounding box editor
* [Bugfix] The code of custom plants were not generated
* [Bugfix] An error was still printed in the console saying custom trees are not supported yet.

## 1.0
* The plugin no longer requires ClothCommons to work
* Updated to MCreator 2021.1.3117
* Updated to Minecraft 1.16.5
* Updated Fabric API to 0.32.0
* Added support for custom potions
* Added support for custom dimensions (no portal)
* Updated the biome, command, food, loot table and overlay to support new features
  //Note for biomes: The biome dictionary is not supported because fabric doesn't support for the moment. Check below for custom trees 
  //Note for foods: When item is dropped and When entity swing item are still not implemented)
* Added support for slab, leaves and pane block bases
* Added support for custom trees in biomes
  //Note: Max water depth, custom vines and fruits are not implemented yet (water depth is not supported)
* Added the smithing recipe type
* Added support for local variables in procedures
* Added crop model for blocks
* Added support for custom block item and particle textures
* Added Is immune to fire, glow condition, recipe remainder, rarity
* Added support for new item stack related procedure blocks: Is enchanted, Is enchantable, Has enchantment, Set number of items to,
  Cooldown for, Get damage, Get enchantment level, Provided itemstack
* Added support for the Return and Console log procedure blocks
* Explode procedure block now supports the explosion type  
* Biomes can now be generated in the overworld
* Added all missing mappings and fixed some mapping files
* Remove mixins entirely
* Custom axes, pickaxes, swords, shovels and hoes have now to be added inside the fabric item tag to work with modded blocks
  //Note: Item tags: fabric:axes, fabric:pickaxes, fabric:swords, fabric:shovels and fabric:hoes
  //Without this change, files have to be manually changed to remove the "null" each type a custom tool is deleted.
* [Bugfix] Mods couldn't be exported
* [Bugfix] Run client could not work
* [Bugfix] Fix transparency parameter for blocks
* [Bugfix] Blocks didn't build properly
* [Bugfix] Tools failed to compile when the attack speed was set to a decimal, and the damage would be reduced by the attack speed.
* [Bugfix] Surely more bug fix caused by mixins
* [Bugfix] Custom armors had a black and white renderer
* [Bugfix] Custom armors without an equipment sound or with an invalid sound caused a build error
* [Bugfix] Number dependencies in procedures couldn't be used
* [Bugfix] Default map color for blocks caused a build error
* [Bugfix] Custom music discs didn't play the sound
* [Bugfix] Fix custom enchantments in mappings

## 1.0.0-pre6
* Updated to the second 2020.5 snapshot
* Started to update biomes to the second 2020.5 snapshot. (Structures and Default Features)
* [Bugfix] Blocks Break Thread Three Fix #74 and #80 

## 1.0.0-pre5
* Added overworld biome generation. 

## 1.0.0-pre4
* Updated to 1.16.3
* [Bugfix] Fixed a crash with modmenu

## 1.0.0-pre3
* Updated to 1.16.3 rc-1
* Re-added modmenu support

## 1.0.0-pre2
* Added Ranged Item mod element.

## 1.0.0-pre1
* Added Plant mod element
* Added Biome mod element
* Added the damage vs mob/animal for items (#68)
* Some mapping changes
* [Bugfix] Fixed Item, Tool and Block Tooltips
* [Bugfix] Fixed block_nbt_num_set
* [Bugfix] Fixed commands (fixes #65)

## 1.0.0-alpha5
- Updated Fabric, Fabric API and mapping versions
- [Bugfix #45]  Procedures didn't compile properly (#57)
- [Bugfix #50] Food elements didn't compile properly (#59)
- Added emissive lighting for blocks (#59)

## 1.0.0-alpha4
The plugins now require [Cloth Commons](https://github.com/ClothCreators/ClothCommons) to work.

* Added all mappings (1.16.2 and before)
* [Bugfix] Fixed x y z dependencies in global triggers
* [Bugfix #47]
* [Bugfix #51]

## 1.0.0-alpha3
- Updated the generator to Minecraft 1.16.2
- [Bugfix #48]

## 1.0.0-alpha2
- Added overlays
- Added music discs
- Added key bindings (They still have bugs)
- Added commands
- Added enchantments
- [Bugfixes] Fixed all (or almost, an option for the items has been deactivated for the moment) elements of the first alpha version.

## 1.0.0-alpha1
- Items (inventory is not supported yet)
- Blocks (block entities are not supported yet)
- Armor
- Tools
- Food
- Fuel
- Item groups
- Procedures (77 procedure blocks, and 4 global triggers)
- Custom code
- Recipes
- Advancements
- Loot tables
- Functions
- Tags

## 0.6.1
* [Bugfix #32]
* [Bugfix #33]
* Updated fabric API

## 0.6.0
### All Changes:-
* **Added support for Non-pushable block entities**
* **Armor can now use custom sounds**
* **Added support for Falling blocks**
* **Item groups are back!**
* **Added support for directional properties on blocks (all five of them)**
* **Added support for custom voxelshapes that work with directional blocks**
* **Added support for custom biomes**
* **Added support for Ore generation. This is very incomplete and  works only in the nether and overworld, and replaces netherrack and the 4 stone variants respectively**
* **Added support for the creation of plants**. Features:
  * Offset type
  * All other implemented block properties
  * Unbreakability
* Added support for Item, Block and Food tooltips
* Added support for enchantment glint on Items and Food
* Added support for drinking on food (drinking means different sounds and no particles)
* Added support for enchantability on Items
* Added support for melee damage on Items
* Added tool tags for tools
* Added support for the luminance on Blocks
* Added support for light opacity on Blocks
* Added the ability to add custom fuels (and it works this time)
* The base mod now includes mod menu
* Food can now have custom eating time
* Updated Loom to 0.4.26
* Added support for block transparency
* Added support for connected block sides
* Added support for block tick rate (Does nothing for now)
* Updated fabric API to 0.12
* Updated yarn version

### Changes from the previous snapshot:-
* Fixed a critical bug with biomes
* Optimized code
* Updated fabric loader to 0.8.8

## 0.5.0
- **Updated Fabric API version to 0.11.1+build.312-1.15**
- **Updated the Fabric version for 0.8.7+build.201 (If you get an error with the setup, Re-run the setup.)**
- Updated yarn mappings for the 1.15.2+build.17 version
- **Added support for armors**
- Added support for the Repair Items feature for Tools and Armors
- Added harvest level for mining blocks
- Not Specified tool can now be used for block.
- Other mapping changes
- [Bugfix] Block hardness didn’t work properly with numbers.
- **[Bugfix #5] Smelting, Blasting, Smoking, Campfire recipe types didn't work.**

## 0.4.1
* [Bugfix] Fixed some block materials having wrong mapping names
* [Bugfix] Fixed block sounds having wrong mapping names
* Added more block materials
* Changed block materials

## 0.4.0
* Added support for tools (Pickaxe, Axe, Shovel, and Sword)
* Added support for the maximal damage for items
* The generator has now its own workspace type. Your old workspaces can be broken. It is recommended to create a new workspace.
* Removed Block Render (Didn't work)
* [Bugfix] Fixed Fuel element
* [Bugfix] The main class had nothing inside if you make a block
* [Bugfix] Fixed Block element

## 0.3.0
* Added Basic Block Element:
  * Render (Solid, cutout, cutout mipped, and translucent)
  * Hardness/Resistance/Material/Sound/Creative tab
  * Generation in the world (Specific biomes don’t work)
* Added Food Element (Few parameters don’t work)
* Added Fuel Element


## 0.2.1
* [Bugfix] Fixed bugs
* Removed ItemGroup feature, will be re-added later
* Added Recipe, Tag, Function, Advancement, and Loot Table Features

## 0.2.0
* Added Basic Creative Tabs
* Added Advancements
* Added Loot Tables
* Added Recipes
* Added Functions
* Added Recipes

## 0.1.0
* Basic item support
