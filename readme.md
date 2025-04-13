![Hardcore lives](https://github.com/user-attachments/assets/b8185960-77bd-4a04-ae03-e2a00de7e3c3)


## O co jde
- Každý hráč má na začátku pouze 3 životy
- Při smrti ztrácí 1 život
- Po ztrátě všech životů je hráč dočasně zabanován (0-10 hodin)
- Po návratu z banu má hráč pouze 1 život
- Zlatá jablka obnovují životy (max. 3)
- Oznámení o banech se zasílají na Discord server

## Příkazy
- `/zivoty` - zobrazí počet zbývajících životů
- `/zivotyvse [stránka]` - zobrazí počet životů všech hráčů včetně offline (aliasy: `/allives`, `/vsezivoty`)
- `/resetlives <hráč>` - obnoví hráči všechny životy (jen admin)
- `/setlives <hráč> <počet>` - nastaví počet životů (jen admin)
- `/testdiscord` - otestuje odesílání zpráv na Discord (jen admin)

## Jak nainstalovat
1. Stáhněte [Skript plugin](https://www.spigotmc.org/resources/skript.114544/)
2. Stáhněte [EssentialsX](https://essentialsx.net/downloads.html)
3. Stáhněte [DiscordSRV](https://www.spigotmc.org/resources/discordsrv.18494/) pro Discord integraci
4. Nakopírujte všechny pluginy do složky `/plugins/`
5. Nakopírujte `hardcore.sk` do složky `/plugins/Skript/scripts/`
6. Restartujte server nebo použijte `/sk reload hardcore.sk`

## Oprávnění
- `lives.admin` - přístup k admin příkazům (`/resetlives`, `/setlives`, `/testdiscord`)
- `lives.list` - přístup k příkazu `/zivotyvse` pro zobrazení životů všech hráčů

## Funkce
### Systém životů
- Hráči mají maximálně 3 životy
- Životy jsou uloženy pomocí UUID, takže fungují i po změně jména
- Při smrti se odečte jeden život
- Barvy životů: zelená (3), oranžová (2), červená (1)

### Obnova životů
- Snědení zlatého jablka přidá jeden život
- Snědení očarovaného zlatého jablka také přidá jeden život
- Maximum je vždy 3 životy
- Při snězení jablka se přehraje zvukový efekt

### Seznam životů
- Příkaz `/zivotyvse` zobrazí přehledný seznam všech hráčů
- Zobrazuje 10 hráčů na stránku s navigací
- Označuje online hráče zelenou barvou
- Barevně rozlišuje počet životů pro lepší přehlednost

### Dočasný ban
- Při ztrátě všech životů je hráč dočasně zabanován
- Náhodná délka banu 1 sekunda až 10 hodin
- Po odbanování se hráč vrací s 1 životem

## Nastavení Discord integrace
1. Vytvořte Discord bota a získejte jeho token
2. Nakonfigurujte DiscordSRV v `/plugins/DiscordSRV/config.yml`:
   - Vložte token vašeho bota
   - Nastavte kanál `server-bany` pro oznámení o banech
3. Restartujte server pro aktivaci Discord integrace
4. Pro ověření fungování použijte příkaz `/testdiscord`

## Komunikace s Discordem
- Při ztrátě všech životů systém automaticky pošle oznámení o banu na Discord
- Zprávy obsahují:
  - Jméno zabanovaného hráče
  - Délku dočasného banu
  - Emoji pro lepší vizuální efekt

## Požadavky
- Spigot/Paper server 1.8+ (testováno na 1.16+)
- Skript plugin v nejnovější verzi
- EssentialsX plugin
- DiscordSRV plugin (pro Discord integraci)

## Řešení problémů
Pokud skript nefunguje:
1. Zkontrolujte verze pluginů
2. Ujistěte se, že server má správná oprávnění
3. Restartujte server

Pokud Discord integrace nefunguje:
1. Zkontrolujte, zda je bot online na vašem Discord serveru
2. Ověřte správné nastavení v config.yml souboru DiscordSRV
3. Zkontrolujte logy v `/plugins/DiscordSRV/debug/` pro případné chyby
4. Zkontrolujte oprávnění bota na Discord serveru
5. Použijte příkaz `/discord reload` pro obnovení připojení

## Poslední aktualizace
- Přidán příkaz `/zivotyvse` pro zobrazení životů všech hráčů včetně offline
- Vylepšena integrace s Discord serverem
- Opraveny chyby ve formátování časů banu
- Aktualizováno: 13. dubna 2025
