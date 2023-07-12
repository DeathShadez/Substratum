# Substratum
![substratum](https://github.com/DeathShadez/Substratum/assets/51402617/8430cc4e-fb97-43df-b5ba-ab6a1170b6ff)

A Terra pack that creates a completely underground world with several unique caves to explore within.

Part of this pack uses resources from these packs:
- OverworldConfig, found [here](https://github.com/PolyhedralDev/TerraOverworldConfig).
- ReimagEnd, found [here](https://github.com/justaureus/ReimagEND).


As of Terra version 6.2, there is no easy way to set generators on the Fabric and Forge platform implementations other than the overworld.  
Due to this, the only platform that you can easily use this pack on is the Bukkit version.  Please keep this in mind before creating issues related to the Fabric or Forge platforms.

## POSSIBLE ISSUES
Might spawn players at the top bedrock layer when used for multiverse custom worlds

## INSTALLATION
Follow this [installation guide](https://terra.polydev.org/install/index.html) for your particular platform.

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
