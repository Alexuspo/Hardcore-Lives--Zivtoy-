# Hardcore Lives System

## About (EN)
- Players start with 3 lives
- Death costs 1 life
- Players with 0 lives are temporarily banned (0-10 hours)
- After ban expires, players return with 1 life
- Golden apples restore lives (max 3)
- Ban notifications sent to Discord

### Commands
- `/lives` - shows remaining lives
- `/alllives [page]` - shows all players' lives (aliases: `/liststats`)
- `/resetlives <player>` - restores all lives (admin only)
- `/setlives <player> <amount>` - sets lives count (admin only)
- `/testdiscord` - tests Discord integration (admin only)

### Installation
1. Install [Skript](https://www.spigotmc.org/resources/skript.114544/), [EssentialsX](https://essentialsx.net/downloads.html) and [DiscordSRV](https://www.spigotmc.org/resources/discordsrv.18494/)
2. Copy `hardcore-en.sk` or `hardcore.sk` to `/plugins/Skript/scripts/`
3. Restart server or use `/sk reload hardcore-en.sk`

### Permissions
- `lives.admin` - admin commands access
- `lives.list` - access to `/alllives` command

### Requirements
- Spigot/Paper server 1.8+
- Updated April 13, 2025

---

## O systému (CZ)
- Hráči začínají se 3 životy
- Při smrti ztrácejí 1 život
- Hráč s 0 životy je dočasně zabanován (0-10 hodin)
- Po vypršení banu se vrací s 1 životem
- Zlatá jablka obnovují životy (max 3)
- Oznámení o banech zasílána na Discord

### Příkazy
- `/zivoty` - zobrazí zbývající životy
- `/zivotyvse [stránka]` - zobrazí životy všech hráčů (aliasy: `/allives`, `/vsezivoty`)
- `/resetlives <hráč>` - obnoví všechny životy (jen admin)
- `/setlives <hráč> <počet>` - nastaví počet životů (jen admin)
- `/testdiscord` - otestuje Discord integraci (jen admin)

### Instalace
1. Nainstalujte [Skript](https://www.spigotmc.org/resources/skript.114544/), [EssentialsX](https://essentialsx.net/downloads.html) a [DiscordSRV](https://www.spigotmc.org/resources/discordsrv.18494/)
2. Zkopírujte `hardcore.sk` nebo `hardcore-en.sk` do `/plugins/Skript/scripts/`
3. Restartujte server nebo použijte `/sk reload hardcore.sk`

### Oprávnění
- `lives.admin` - přístup k admin příkazům
- `lives.list` - přístup k příkazu `/zivotyvse`

### Požadavky
- Spigot/Paper server 1.8+
- Aktualizováno 13. dubna 2025
