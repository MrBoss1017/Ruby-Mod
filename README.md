# RUBY MOD

A modern vanilla-plus equipment and mineral tier for Fabric 26.3.

![Minecraft](https://img.shields.io/badge/Minecraft-26.3-70a93c?style=flat-square)
![Loader](https://img.shields.io/badge/Loader-Fabric-dbb17e?style=flat-square)
![Java](https://img.shields.io/badge/Java-25-ea7500?style=flat-square)
![License](https://img.shields.io/badge/License-GPL--3.0--only-845ec2?style=flat-square)

---

## Overview

**Ruby Mod** expands vanilla Minecraft progression by introducing subterranean ruby minerals, decorative storage blocks, and a dedicated tier of ruby tools and armor. Built natively for Fabric 26.3 with pure lightweight mechanics—no extra GUIs, no custom keybinds, and zero commands required.

---

## Features

### Minerals & Blocks
* **Ruby Ore:** Found rarely in stone layers at intermediate and deep elevations.
* **Deepslate Ruby Ore:** Denser vein generation embedded within deepslate strata.
* **Ruby Gem:** The core crafting component dropped from mined ores or smelted raw materials.
* **Block of Ruby:** High-luster storage and decorative block crafted from nine Ruby Gems.

### Equipment & Tools
* **Ruby Armor Set:** Helmet, Chestplate, Leggings, and Boots providing high durability and armor toughness.
* **Ruby Toolset:** Sword, Pickaxe, Axe, Shovel, and Hoe configured with high harvest speed and durability.

---

## Item & Equipment Reference

| Category | Items | Primary Material | Notes |
| :--- | :--- | :--- | :--- |
| **Minerals** | Ruby Gem | — | Core component; obtained via mining or smelting |
| **Blocks** | Ruby Ore, Deepslate Ruby Ore, Block of Ruby | Stone / Deepslate / Ruby | Requires Iron Pickaxe or better to harvest |
| **Armor** | Helmet, Chestplate, Leggings, Boots | Ruby Gem | High-tier protection & durability |
| **Tools** | Sword, Pickaxe, Axe, Shovel, Hoe | Ruby Gem + Sticks | High attack damage and mining efficiency |

---

## Configuration

Custom balance parameters are saved under `config/rubymod.json`. Values can be edited directly while the server or singleplayer instance is offline.

```json
{
  "oreGeneration": {
    "rubyVeinSize": 6,
    "veinsPerChunk": 4,
    "minHeight": -64,
    "maxHeight": 32
  },
  "toolStats": {
    "miningSpeed": 9.0,
    "durability": 1800
  },
  "armorStats": {
    "defensePoints": {
      "helmet": 3,
      "chestplate": 8,
      "leggings": 6,
      "boots": 3
    },
    "toughness": 2.5
  }
}
