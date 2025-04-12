# Hardcore Lives System

## O co jde
- Každý hráč má 3 životy
- Při smrti ztrácí 1 život
- Po ztrátě všech životů je hráč dočasně zabanován (0-10 hodin)
- Po návratu z banu má hráč pouze 1 život
- Zlatá jablka obnovují životy (max. 3)

## Příkazy
- `/zivoty` - zobrazí počet zbývajících životů
- `/resetlives <hráč>` - obnoví hráči všechny životy (jen admin)
- `/setlives <hráč> <počet>` - nastaví počet životů (jen admin)

## Jak nainstalovat
1. Stáhněte [Skript plugin](https://www.spigotmc.org/resources/skript.114544/)
2. Stáhněte [EssentialsX](https://essentialsx.net/downloads.html)
3. Nakopírujte oba pluginy do složky `/plugins/`
4. Nakopírujte `hardcore.sk` do složky `/plugins/Skript/scripts/`
5. Restartujte server nebo použijte `/sk reload hardcore.sk`

## Požadavky
- Spigot/Paper server
- Skript plugin
- EssentialsX plugin

## Řešení problémů
Pokud skript nefunguje:
1. Zkontrolujte verze pluginů
2. Ujistěte se, že server má správná oprávnění
3. Restartujte server