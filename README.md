# Substratum
![substratum](https://github.com/DeathShadez/Substratum/assets/51402617/6774bb7a-f23a-47e8-aa32-d88870293da9)


A Terra pack that creates a completely underground world with several unique caves to explore within.

Part of this pack uses resources from these packs:
- OverworldConfig, found [here](https://github.com/PolyhedralDev/TerraOverworldConfig).
- ReimagEnd, found [here](https://github.com/justaureus/ReimagEND).

## POSSIBLE ISSUES
- Might spawn players at the top bedrock layer depending on how world is generated
- Players might spawn and suffocate upon initial spawn

## Installation
Download the Substratum pack from the [releases page](https://github.com/DeathShadez/Substratum/releases) for a reliable pack version 
or from the main Substratum branch for changes that haven't been applied to the latest release yet.

### Read the *World Installation* section if you want a typical fully underground Substratum world. 
### Otherwise skip ahead to the *Drop-In Merge Installation* section for adding Substratum caves to other packs. 

## World Installation
Follow this [installation guide](https://terra.polydev.org/install/index.html) for your particular platform.

Fabric users will have to edit the `level.dat` in order to apply custom generation to the end dimension.

#### Bukkit.yml Quick Reference For Overworld
##### For custom worlds, replace "world" with your custom world name
```
worlds:
  world:
    generator: Terra:SUBSTRATUM
```
##### More than One Config Pack for Multiple Worlds 
```
worlds:
  world:
    generator: Terra:OVERWORLD
  world_name:
    generator: Terra:SUBSTRATUM
```

## Drop-In Merge Installation
If you want to add Substratum's cave biomes to a pack, *please follow the steps below closely*.

1. Copy all of Substratum's content over to the desired pack 
##### Substratum content being *EVERYTHING* including the folders and the pack.yml.

2. Ensure that duplicate files are ignored and skipped

3. Go to the `substratum_meta.yml` and edit the max and min values for cave biomes to your desired pack values.

4. Go to the preset for your desired pack (default overworld config is `TerraOverworldConfig\biome-providers\presets\default.yml`)
and add `- << biome-providers/extrusions/add_substratum_cave_biomes.yml:extrusions` to the extrusions list.

## How to Disable Biomes
Dislike a particular cave biome? 
Well, you can customize everything in Substratum to your liking and that includes disabling any cave biomes!
##### Go to the `Substratum\biome-providers\extrusions\add_substratum_cave_biomes.yml` and comment out the biome
###### Place a # in front of the weighted item representing the biome in the list to comment out the biome and disable it
