# Opengens Revival

> *"really think shutting it down? will stop me?"* — aquaair

A 1:1 recreation of the original **Opengens** Minecraft server, preserved and revived by aquaair.

---

## What is Opengens?

Opengens was a Minecraft gens (generators) PVP server. Players mined and compressed ores from generators, used their earnings to buy upgrades, and dominated the leaderboard — all while fighting other players for supremacy.

The original server was owned by **voided** (ematthew1) and co-owned by **atlas** (jpgy). When it shut down, it left behind a community that clearly wasn't ready to let it go.

This repository is an effort to bring it back as close to the original as possible.

---

## What's Included

| Asset | Description |
|---|---|
| `texture_pack/` | The original Opengens resource/texture pack |
| `skripts/full_trims.sk` | Custom full armor trim shop (netherite upgrade material, GUI-based) |
| `skripts/combat_tag.sk` | Combat tagging system — log during combat and you die + get banned 5 minutes |
| `skripts/pvp_system.sk` | Bow block at spawn, PVP toggle, region-based PVP enforcement |

---

## Server Features

- **Ore Generators** — Mine, compress, and upgrade your way to the top
- **PVP Zone (Gens area)** — Full PVP enabled, no toggling off
- **Safe Spawn** — PVP disabled, bows blocked *(yes, we will tell you "nice try dipshit")*
- **Full Armor Trims** — Buy custom netherite upgrade trims that cover your entire armor set
- **Combat Logging Protection** — Disconnect mid-fight and face the consequences
- **Per-player PVP Toggle** — Opt in or out of PVP outside of forced zones
- **Free Speech** — No chat filter. Say what you want.

---

## Setup

### Requirements

- [Paper](https://papermc.io/) (1.20.x recommended)
- [Skript](https://github.com/SkriptLang/Skript)
- [SkBee](https://github.com/ShaneBeee/SkBee) — for armor trim NBT
- [Skript-WorldGuard](https://github.com/Pikachu920/skript-worldguard) — for region detection
- [Skript-Vault](https://github.com/Pikachu920/skript-vault) — for economy integration
- [WorldGuard](https://enginehub.org/worldguard/) — define `spawn` and `gens` regions
- A temp-ban plugin — [LiteBans](https://www.spigotmc.org/resources/litebans.3715/) recommended

### Installation

1. Clone this repo or download as ZIP
2. Drop the `.sk` files into your server's `plugins/Skript/scripts/` folder
3. Add the texture pack to your server's resource pack slot (server.properties or a resource pack plugin)
4. Define two WorldGuard regions on your server:
   - `spawn` — your spawn area (PVP off, bows blocked)
   - `gens` — your generators/PVP area (PVP always on)
5. Run `/skript reload all` in-game or restart the server
6. Open `/trimshop` to test the trim GUI

---

## Credits

### Original Server
| Role | Username |
|---|---|
| Owner | voided (ematthew1) |
| Co-Owner | atlas (jpgy) |

### Revival
| Role | Username |
|---|---|
| Owner & Developer | aquaair |

---

## License

This project is licensed under the **Apache License 2.0**.
See [LICENSE](./LICENSE) for details.

You're free to use, modify, and distribute this — just give credit.

---

*Opengens lives.*
