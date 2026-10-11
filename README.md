# RUBY MOD

A precision vanilla-plus equipment and subterranean mineral tier for Minecraft 26.3.

![Minecraft](https://img.shields.io/badge/Minecraft-26.3-70a93c?style=flat-square)
![Loader](https://img.shields.io/badge/Loader-Fabric-dbb17e?style=flat-square)
![Java](https://img.shields.io/badge/Java-25-ea7500?style=flat-square)
![License](https://img.shields.io/badge/License-GPL--3.0--only-845ec2?style=flat-square)
![Build](https://img.shields.io/badge/build-passing-brightgreen?style=flat-square)

[Overview](#overview) • [World Generation](#world-generation) • [Equipment & Tools](#equipment--tools) • [Blockset](#the-blockset) • [Configuration](#configuration) • [Download & Installation](#download--installation) • [Building from Source](#building-from-source) • [Source Map](#source-map-and-contributing)

---

## Overview

**Ruby Mod** seamlessly expands vanilla Minecraft progression by introducing deep subterranean ruby deposits, dense deepslate variants, decorative storage blocks, and an endgame-ready tier of ruby tools and armor. Built natively for **Fabric 26.3**, the mod enforces a clean, unobtrusive philosophy:

* **Zero Commands:** Everything is discovered and acquired naturally through vanilla exploration and crafting.
* **Zero Custom Keybinds:** Relies purely on standard Minecraft input schemes.
* **Zero UI Bloat:** Integrates into native inventories, crafting grids, smithing benches, and creative tabs.
* **Deterministic Server Authority:** Ore generation, tool durability, combat calculations, and harvesting checks remain strictly authoritative on the server or internal host.

---

## What Ruby Mod Brings to Minecraft

* **Subterranean Stratification:** Separate stone and deepslate vein profiles tuned to prevent early-game exploitation while rewarding deep cave exploration.
* **Full Defensive Ensemble:** Four-piece armor set positioned between Diamond and Netherite tiers, featuring elevated armor toughness and high baseline durability.
* **High-Efficiency Harvesting:** Complete five-piece toolset (Sword, Pickaxe, Axe, Shovel, Hoe) offering high mining multipliers and balanced attack curves.
* **Compact Block Storage:** Nine-gem compression into gleaming decorative blocks with beacon base support.
* **Zero Runtime Overhead:** Pure Java 25 / Fabric API architecture without heavy external runtime dependencies, shaders, or rendering hooks.

---

## World Generation

Ruby veins generate naturally in the Overworld through standard vanilla biome feature injections. Generation profiles are configured to spawn sparingly in standard stone layers and more frequently throughout deep slate levels.

| Mineral Node | Primary Stratum | Target Y-Levels | Default Vein Size | Veins / Chunk | Harvest Tier |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Ruby Ore** | Stone | Y: 0 to Y: 32 | 4–6 blocks | 3 | Iron Pickaxe+ |
| **Deepslate Ruby Ore** | Deepslate / Tuff | Y: -64 to Y: 0 | 6–8 blocks | 5 | Iron Pickaxe+ |

*Note: Ruby veins obey Silk Touch and Fortune enchantment scaling. Without Silk Touch, breaking ore drops raw Ruby Gems alongside experience orbs.*

---

## Equipment & Tools

### Armor Set

Designed as an alternative to Diamond armor, Ruby Armor focuses on exceptional durability and elevated knockback / toughness resistance.

| Armor Piece | Defense (Armor Points) | Armor Toughness | Knockback Resistance | Baseline Durability |
| :--- | :--- | :--- | :--- | :--- |
| **Ruby Helmet** | +3 | +2.0 | +0.05 | 360 |
| **Ruby Chestplate** | +8 | +2.5 | +0.10 | 520 |
| **Ruby Leggings** | +6 | +2.0 | +0.05 | 490 |
| **Ruby Boots** | +3 | +2.0 | +0.05 | 420 |
| **Full Set Total** | **20 Points** | **+8.5 Toughness** | **+0.25 Resistance** | — |

---

### Toolset

Ruby tools feature a mining speed that matches or slightly exceeds Diamond, while retaining high baseline durability suitable for long-term mining sessions.

| Tool | Attack Damage | Attack Speed | Mining Multiplier | Harvest Tier | Durability |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Ruby Sword** | 7.5 | 1.6 | 1.5x | — | 1,750 |
| **Ruby Pickaxe** | 5.0 | 1.2 | 9.0x | Level 3 (Diamond equiv.) | 1,750 |
| **Ruby Axe** | 9.0 | 0.9 | 9.0x | Level 3 | 1,750 |
| **Ruby Shovel** | 4.5 | 1.0 | 9.0x | Level 3 | 1,750 |
| **Ruby Hoe** | 1.0 | 4.0 | 9.0x | Level 3 | 1,750 |

---

## The Blockset

* **Block of Ruby:**
  * **Crafting Recipe:** 9x Ruby Gems arranged in a 3×3 crafting table grid.
  * **Blast Resistance:** 6.0
  * **Hardness:** 5.0
  * **Beacon Compatibility:** Acts as a valid pyramid base block.
* **Deepslate Ruby Ore:**
  * **Blast Resistance:** 6.0
  * **Hardness:** 4.5
  * Drops 1x Ruby Gem (scaled with Fortune I–III) and 3–7 experience points.

---

## Configuration

Custom world balance, vein distribution, and equipment properties are managed via a single human-readable JSON file located at `config/rubymod.json`. The file is created automatically on the first server/client run.

```json
{
  "generation": {
    "enableOreGen": true,
    "stoneVeinSize": 6,
    "stoneVeinsPerChunk": 3,
    "deepslateVeinSize": 8,
    "deepslateVeinsPerChunk": 5,
    "minY": -64,
    "maxY": 32
  },
  "toolStats": {
    "durabilityMultiplier": 1.0,
    "miningSpeed": 9.0,
    "damageBonus": 3.5
  },
  "armorStats": {
    "durabilityMultiplier": 1.0,
    "toughness": 2.5,
    "knockbackResistance": 0.05
  }
}
