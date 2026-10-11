<p align="center">
  <img width="3584" height="1184" alt="banner" src="https://github.com/user-attachments/assets/362bf073-854f-4643-ad81-fd1bca58994d" />
</p>

<p align="center">
  <h3 align="center">The Earth is the weapon.</h3>
</p>

<p align="center">
  <strong>A subterranean mineral tier. A forged arsenal. A world that yields to the pickaxe.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Minecraft-26.3-70a93c?style=flat-square" alt="Minecraft 26.3">
  <img src="https://img.shields.io/badge/Loader-Fabric-dbb17e?style=flat-square" alt="Fabric Loader">
  <img src="https://img.shields.io/badge/Java-25-ea7500?style=flat-square" alt="Java 25">
  <img src="https://img.shields.io/badge/License-GPL--3.0--only-845ec2?style=flat-square" alt="GPL-3.0-only">
  <img src="https://img.shields.io/badge/build-passing-brightgreen?style=flat-square" alt="Build Passing">
</p>

<p align="center">
  <a href="#installation">Installation</a> • 
  <a href="#equipment">Equipment</a> • 
  <a href="#worldgen">Worldgen</a> • 
  <a href="#blockset">Blockset</a> • 
  <a href="#configuration">Configuration</a> • 
  <a href="#building-from-source">Building from Source</a>
</p>

<p align="center">
  <a href="https://github.com/MrBoss1017/Ruby-Mod/releases/latest"><strong>Download Ruby Mod v1.0.0</strong></a>
</p>

---

## Overview

**Ruby Mod: The Red Stratum** is an authentic vanilla-plus Fabric mod for **Minecraft 26.3** that introduces subterranean ruby minerals, dense deepslate variants, decorative storage blocks, and an endgame-ready tier of ruby tools and armor. Built natively for Fabric with a clean, unobtrusive philosophy:

* **Zero Custom Commands:** All ores, gems, and forged gear are discovered and crafted naturally through vanilla survival progression.
* **Zero Custom Keybinds:** Fully compatible with default keyboard, mouse, and gamepad profiles without reserved keybind conflicts.
* **Zero UI Bloat:** Integrates into native inventories, crafting tables, anvils, and creative tabs without extra HUD overlays or screen clutter.
* **Deterministic Server Authority:** Ore distribution, durability depletion, damage scaling, and block harvesting belong strictly to the server host.

---

## What Ruby Mod Brings to Minecraft

* **Subterranean Stratification:** Separate stone and deepslate vein generation profiles tuned to reward deep exploration without saturating early cave systems.
* **Full Defensive Ensemble:** Four-piece armor set positioned between Diamond and Netherite with elevated armor toughness and knockback mitigation.
* **Precision Harvest Suite:** Full five-piece toolset (Sword, Pickaxe, Axe, Shovel, Hoe) offering high mining multipliers and balanced attack curves.
* **Decorative Compression:** Nine-gem compact storage blocks with native beacon pyramid foundation support.
* **Zero Runtime Overhead:** Pure Java 25 / Fabric API architecture without heavy external runtime dependencies, custom shaders, or rendering hooks.

---

## Download

Direct release packages are distributed as compressed archives containing the production mod binary and default server configuration templates.

* **Latest Release:** [Download ruby_mod-1.0.0.zip](https://github.com/MrBoss1017/Ruby-Mod/releases/latest)
* **Archive Name:** `ruby_mod-1.0.0.zip`

### Extracted Directory Contents
Extracting `ruby_mod-1.0.0.zip` yields the following production structure:

ruby_mod-1.0.0/
├── rubymod-1.0.0.jar             # Compiled production mod binary
└── config/
└── rubymod.json              # Default server/client configuration template

---

## <a id="installation"></a>Installation

### Singleplayer Client
1. Install **Fabric Loader** for **Minecraft 26.3** via the official Fabric installer.
2. Download the matching **Fabric API** build for Minecraft 26.3.
3. Download and extract **`ruby_mod-1.0.0.zip`** to reveal `ruby_mod-1.0.0/`.
4. Open your Minecraft root directory:
   * **Windows:** Press `Win + R`, type `%appdata%\.minecraft`, and press **Enter**.
   * **macOS:** Navigate to `~/Library/Application Support/minecraft`.
   * **Linux:** Navigate to `~/.minecraft`.
5. Open the `mods` folder (create one if it does not exist) and copy **`rubymod-1.0.0.jar`** into it alongside `fabric-api.jar`.
6. *(Optional)* Copy the extracted `config/rubymod.json` into `.minecraft/config/rubymod.json` to customize values before first launch. If omitted, default values generate automatically.
7. Launch Minecraft using your Fabric 26.3 profile.

### Dedicated Multiplayer Server
1. Prepare a clean **Fabric 26.3** dedicated server instance.
2. Ensure **Java 25** is set up in your server execution path (`java -version`).
3. Place `fabric-api.jar` and `rubymod-1.0.0.jar` into the server's root `mods/` directory.
4. Place the default `config/rubymod.json` into the server's root `config/` directory, or start the server once to generate defaults automatically.
5. Boot the server via your launch script.

---

## <a id="equipment"></a>The Arsenal & Equipment

The equipment tier bridges the power progression gap between pristine Diamond gear and Netherite upgrades, prioritizing durability longevity and high baseline toughness.

### Armor Specifications

| Armor Piece | Defense (Armor Points) | Armor Toughness | Knockback Resistance | Baseline Durability | Repair Material |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Ruby Helmet** | +3 Points | +2.0 Toughness | +0.05 (5%) | 360 Durability | Ruby Gem |
| **Ruby Chestplate** | +8 Points | +2.5 Toughness | +0.10 (10%) | 520 Durability | Ruby Gem |
| **Ruby Leggings** | +6 Points | +2.0 Toughness | +0.05 (5%) | 490 Durability | Ruby Gem |
| **Ruby Boots** | +3 Points | +2.0 Toughness | +0.05 (5%) | 420 Durability | Ruby Gem |
| **Full Set Total** | **20 Points** | **+8.5 Toughness** | **+0.25 (25%)** | **1,790 Total** | — |

### Toolset Specifications

Ruby tools feature an aggressive mining speed multiplier matching or exceeding Diamond gear while providing sustained work time in survival scenarios.

| Tool | Attack Damage | Attack Speed | Mining Multiplier | Harvest Tier | Baseline Durability | Anvil Repair |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Ruby Sword** | 7.5 Damage | 1.6 Attacks/s | 1.5x Speed | — | 1,750 | Ruby Gem |
| **Ruby Pickaxe** | 5.0 Damage | 1.2 Attacks/s | 9.0x Speed | Level 3 (Diamond equiv.) | 1,750 | Ruby Gem |
| **Ruby Axe** | 9.0 Damage | 0.9 Attacks/s | 9.0x Speed | Level 3 (Diamond equiv.) | 1,750 | Ruby Gem |
| **Ruby Shovel** | 4.5 Damage | 1.0 Attacks/s | 9.0x Speed | Level 3 (Diamond equiv.) | 1,750 | Ruby Gem |
| **Ruby Hoe** | 1.0 Damage | 4.0 Attacks/s | 9.0x Speed | Level 3 (Diamond equiv.) | 1,750 | Ruby Gem |

### Enchantment & Anvil Mechanics
* **Enchantability:** Tools and armor feature an enchantability rating of 12, allowing access to top-tier enchantment rolls on enchanting tables.
* **Anvil Restorations:** Combining worn tools or armor pieces with raw **Ruby Gems** restores 25% of baseline durability per gem expended.
* **Mending & Unbreaking:** Full native compatibility with vanilla enchantment books without requiring custom tags.

---

## <a id="worldgen"></a>World Generation

Ruby mineral features are injected directly into Overworld chunk generator pipelines during the subterranean generation pass. Placement rules maintain strict separation between the upper stone shell and the lower deepslate foundation.

### Mineral Stratification

| Mineral Node | Host Stratum | Elevation Range (Y) | Default Vein Size | Placement Attempts / Chunk | Harvest Requirement |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Ruby Ore** | Stone | Y: 0 to Y: 32 | 4–6 blocks | 3 passes | Iron Pickaxe or higher |
| **Deepslate Ruby Ore** | Deepslate / Tuff | Y: -64 to Y: 0 | 6–8 blocks | 5 passes | Iron Pickaxe or higher |

### Drop & Extraction Rules
* **Standard Harvest:** Mined without Silk Touch, breaking ore drops 1x Ruby Gem and grants 3–7 experience points.
* **Fortune Scaling:** Fortune I–III increases the maximum gem drop count up to 4 gems per block.
* **Silk Touch Harvesting:** Drops the intact ore block (`rubymod:ruby_ore` or `rubymod:deepslate_ruby_ore`), which can be smelted in a Furnace or Blast Furnace to produce 1x Ruby Gem.

---

## <a id="blockset"></a>The Blockset

The mod introduces solid mineral blocks for compact storage, base construction, and beacon power arrays.

### Block Definitions

* **Block of Ruby (`rubymod:ruby_block`):**
  * **Crafting Pattern:** 9x Ruby Gems filled across all 9 slots of a crafting table.
  * **Blast Resistance:** 6.0
  * **Hardness Value:** 5.0
  * **Beacon Compatibility:** Acts as a valid foundation pyramid block for tier 1–4 Beacon towers.
  * **Flammability:** Non-flammable / lava immune.
* **Ruby Ore (`rubymod:ruby_ore`):**
  * **Blast Resistance:** 3.0
  * **Hardness Value:** 3.0
  * **Tool Required:** Iron Pickaxe or better.
* **Deepslate Ruby Ore (`rubymod:deepslate_ruby_ore`):**
  * **Blast Resistance:** 6.0
  * **Hardness Value:** 4.5
  * **Tool Required:** Iron Pickaxe or better.

---

## <a id="configuration"></a>Server Configuration

Server administrators and singleplayer worlds can adjust generation rates and equipment parameters via `config/rubymod.json`. The file is created automatically on first launch.

### Configuration Schema (`config/rubymod.json`)

``json
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

---

### Parameter Reference

| Parameter | Category | Data Type | Default | Description |
| :--- | :--- | :--- | :--- | :--- |
| `enableOreGen` | Generation | Boolean | `true` | Master switch for Overworld ruby vein generation |
| `stoneVeinSize` | Generation | Integer | `6` | Maximum block size for standard stone veins |
| `stoneVeinsPerChunk` | Generation | Integer | `3` | Generation passes attempted per chunk between Y: 0 and Y: 32 |
| `deepslateVeinSize` | Generation | Integer | `8` | Maximum block size for deepslate veins |
| `deepslateVeinsPerChunk` | Generation | Integer | `5` | Generation passes attempted per chunk between Y: -64 and Y: 0 |
| `minY` | Generation | Integer | `-64` | Lowest world coordinate where veins can generate |
| `maxY` | Generation | Integer | `32` | Highest world coordinate where veins can generate |
| `durabilityMultiplier` | Equipment | Float | `1.0` | Global scaling factor applied to tool and armor health |
| `miningSpeed` | Tools | Float | `9.0` | Multiplier applied when breaking eligible harvest blocks |
| `toughness` | Armor | Float | `2.5` | Baseline armor toughness granted per heavy armor piece |

---

### Requirements & Compatibility Matrix

| Dependency / Tool | Version | Status | Notes |
| :--- | :--- | :--- | :--- |
| **Minecraft** | 26.3 | Required | Target client and dedicated server runtime |
| **Fabric Loader** | 0.16.x+ | Required | Primary mod initialization environment |
| **Java** | 25 | Required | Minimum JDK/JRE runtime requirement |
| **Fabric API** | 26.3 Compatible | Required | Core hook and registry abstraction layer |
| **Mod Menu** | Compatible | Optional | Supported for client environment inspection |

---

## Building from Source

### Prerequisites
* **Java 25 JDK** installed locally with `JAVA_HOME` pointing to its installation directory.
* Git installed and available on your system path.

### Build Instructions

#### Windows (PowerShell)
powershell
git clone [https://github.com/MrBoss1017/Ruby-Mod.git](https://github.com/MrBoss1017/Ruby-Mod.git)
Set-Location Ruby-Mod
.\gradlew.bat clean build

---

#### Linux / MacOS (Bash)
git clone [https://github.com/MrBoss1017/Ruby-Mod.git](https://github.com/MrBoss1017/Ruby-Mod.git)
cd Ruby-Mod
chmod +x ./gradlew
./gradlew clean build

---

### Release Verification & Artifacts

All production releases undergo automated gradle verification before tagging:

| Target Artifact | Checksum / Target | Environment | Target Status |
| :--- | :--- | :--- | :--- |
| `rubymod-1.0.0.jar` | Production Binary | Minecraft 26.3 / Fabric | Verified Build |
| `ruby_mod-1.0.0.zip` | Release Bundle | Full Distribution | Verified Archive |
| `rubymod.json` | Config Template | Default Spec | Verified Deserialization |

---

## Repository Architecture
Ruby-Mod/
├── .github/
│   └── workflows/                    # Automated CI build pipelines
├── src/
│   └── main/
│       ├── java/com/rubymod/
│       │   ├── RubyMod.java          # Mod initialization and registry hooks
│       │   ├── block/                # Block registry (Ruby Block, Ores)
│       │   ├── item/                 # Equipment, tool, and material registries
│       │   ├── config/               # JSON config loader and serializer
│       │   └── worldgen/             # Configured and Placed Feature rules
│       └── resources/
│           ├── fabric.mod.json       # Mod metadata
│           ├── assets/rubymod/       # Models, blockstates, textures, and lang files
│           └── data/rubymod/         # Worldgen JSONs, tags, recipes, and loot tables
├── gradle/wrapper/                   # Gradle distribution wrapper
├── build.gradle                      # Build and Fabric Loom dependencies
└── settings.gradle                   # Gradle project settings

---

License and credits
Copyright © 2026 MrBoss1017 and Ruby Mod contributors.

Original Ruby Mod code, generated assets, and project documentation are licensed under GNU GPL version 3 only (GPL-3.0-only). See LICENSE for full terms and NOTICE for scope/provenance. Modified covered distributions must meet GPLv3's source and licensing requirements.

Gradle wrapper components and pre-existing template material retain their own notices. Minecraft, Fabric, Mod Menu, Python dependencies, and GitHub Actions are external projects and are not relicensed here. The former template CC0 text is preserved in licenses/CC0-1.0.txt.

Ruby Mod is independent and is not an official Minecraft product or approved by Mojang or Microsoft.
