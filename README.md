# Root-Economy

RootMC Gold economy (Vault, treasury, bonds, loans, upkeep)

| Field | Value |
|-------|-------|
| **Folder / artifact** | `root-economy` |
| **Version** | `1.7.7` |
| **Bukkit name** | `Root-Economy` |
| **Paper API** | `26.1` |
| **Author** | Root Record |
| **Website** | https://rootmc.net |
| **Main class** | `com.rootrecord.minecraft.rooteconomy.RootEconomyPlugin` |

## Install

1. Install **[Root-Core](https://github.com/RootRecord/root-core)** first (license/cloud spine for the suite).
2. Download `root-economy-1.7.7.jar` from [Releases](https://github.com/RootRecord/root-economy/releases) or the [plugin catalog](https://rootmc.net/plugins/).
3. Remove any older `root-economy-*.jar` from `plugins/`.
4. Drop the new jar into `plugins/` and restart (or use Root-Core suite updater when this plugin is on the public manifest).
5. Shared config and secrets live under `plugins/RootMC/` (not a per-plugin data folder unless documented otherwise).

### Dependencies

| Type | Plugins |
|------|---------|
| Hard depend | _none_ |
| Soft depend | Root-Core, Root-Times, Root-Perms, RootMC, Vault, Towny, PlaceholderAPI |

## Configuration

Most RootMC plugins store operator YAML under `plugins/RootMC/`. After first boot, check that folder for new keys. Never commit live `cloud.yml` / database passwords to git.

## Build (monorepo)

Primary compilation is the RootMC Gradle workspace (not this standalone repo alone):

```bat
cd "D:\.1 Work Stations\RootMC\Plugin Building\Minecraft"
.\build-with-server-jdk.bat :plugins:root-economy:jar
```

This repository mirrors sources for GitHub browsing and release distribution. It depends on `rootrecord-common` inside the monorepo.

## Commands (summary)

| Command | Description |
|---------|-------------|
| `/balance` | Show balance |
| `/pay` | Pay another player or donate to the Server Reserve |
| `/paytoggle` | Toggle accepting payments |
| `/baltop` | Balance leaderboard (players; towns/nations on Towny) |
| `/reserve` | Server treasury reserve stats (balance, inflows/outflows, playtime) |
| `/totals` | Precomputed economy list totals (entry types, Towny intake, supply, pools) |
| `/economy` | Total economy (Notes vs gold mined), inflation pressure, and tax info |
| `/tax` | Live transaction tax rate (dynamic while Notes are over-issued) |
| `/mint` | Convert gold items to G, or withdraw G as gold items |
| `/grant` | Grant G from treasury to a player (logged) |
| `/bonds` | Bond vault â€” issue bonds, collect compounding yield, redeem notes in full |
| `/rootbonds` | Admin reload for Root-Bonds |
| `/loan` | Borrow, view, or repay a personal loan |
| `/townloan` | Mayor â€” borrow from Server Reserve into town bank, or repay |
| `/rootloans` | Admin reload for Root-Loans |
| `/rootupkeep` | Admin controls for inactivity tax |

Full command and permission tables: [docs/COMMANDS.md](docs/COMMANDS.md).

## Links

| Resource | URL |
|----------|-----|
| Website | https://rootmc.net |
| Plugin catalog | https://rootmc.net/plugins/ |
| This plugin page | https://rootmc.net/plugins/root-economy/ |
| Suite wiki | https://rootmc.net/wiki/plugins/ |
| Player wiki | https://rootmc.net/wiki/player/ |
| Constitution | https://rootmc.net/wiki/constitution/ |
| Economy guide | https://rootmc.net/wiki/economy/ |
| Developer keys | https://rootmc.net/developer/keys/ |
| Manifest | https://rootmc.net/plugins/manifest.json |
| Play | `play.rootmc.net` |
| Live map | https://map.rootmc.net |
| API | https://api.rootmc.net |
| Discord | https://discord.gg/rFFQYrNaqS |
| GitHub (this repo) | https://github.com/RootRecord/root-economy |
| Releases | https://github.com/RootRecord/root-economy/releases |

**Discord:** RootMC community - join for support, announcements, and governance: https://discord.gg/rFFQYrNaqS


## Documentation in this repo

- [docs/COMMANDS.md](docs/COMMANDS.md) - commands and permissions from `plugin.yml`
- [docs/LINKS.md](docs/LINKS.md) - canonical RootMC web and Discord links
- [CHANGELOG.md](CHANGELOG.md) - version history seed

## License

Copyright Root Record. All rights reserved. Source is published for transparency; no license to copy, modify, or redistribute is granted unless Root Record provides written permission.

