# Hardcore Lives System - Uživatelská příručka

## O systému
Tento plugin přidává do Minecraft serveru systém omezených životů, kde každý hráč má maximálně 3 životy. Když hráč vyčerpá všechny své životy, je dočasně vyloučen ze hry (ban) na náhodnou dobu. Systém také umožňuje získat zpět životy pomocí zlatých jablek.

## Funkce a vlastnosti
- **Omezený počet životů**: Každý hráč má maximálně 3 životy
- **Barevné indikátory**: Životy jsou barevně označeny (zelená pro 3, oranžová pro 2, červená pro 1)
- **Dočasné vyloučení**: Po ztrátě všech životů je hráč dočasně vyloučen ze hry na náhodnou dobu (0-10 hodin)
- **Obnova životů**: Životy lze získat zpět snědením zlatého jablka
- **Zobrazení v TAB menu**: Počet životů se zobrazuje u jména hráče v seznamu hráčů
- **Admin příkazy**: Pro správu životů hráčů

## Základní pravidla
1. Každý hráč začíná se 3 životy
2. Při smrti ztrácíš 1 život
3. Když ztratíš všechny 3 životy, budeš dočasně vyloučen(a) ze serveru
4. Zlatá jablka ti mohou obnovit životy (maximálně do 3)
5. Po návratu na server po vyloučení získáš opět 3 životy

## Hráčské příkazy
| Příkaz | Popis |
|--------|-------|
| `/zivoty` | Zobrazí počet tvých zbývajících životů |

## Obnova životů pomocí zlatých jablek
- **Běžné zlaté jablko**: Obnoví 1 život (až do maxima 3 životů)
- **Očarované zlaté jablko**: Obnoví 1 život (až do maxima 3 životů)

## Barevné značení životů
- **Zelená (3 životy)**: Plný počet životů
- **Oranžová (2 životy)**: Střední riziko
- **Červená (1 život)**: Vysoké riziko - buď opatrný!

## Indikátory v TAB menu
V seznamu hráčů (po stisknutí klávesy TAB) uvidíš u každého jména barevně označený počet životů:
```
Hráč [3]  - zelené číslo
Hráč [2]  - oranžové číslo
Hráč [1]  - červené číslo
```

## Administrátorské příkazy
| Příkaz | Popis | Oprávnění |
|--------|-------|-----------|
| `/resetlives <hráč>` | Obnoví hráči plný počet životů (3) | `lives.admin` |
| `/setlives <hráč> <počet>` | Nastaví hráči specifický počet životů (0-3) | `lives.admin` |

## Tipy pro přežití
1. **Buď opatrný**: Každá smrt tě přibližuje k dočasnému vyloučení
2. **Sbírej zlatá jablka**: Jsou vzácná, ale mohou ti zachránit život
3. **Sleduj počet svých životů**: V TAB menu nebo pomocí příkazu `/zivoty`
4. **Vyhýbej se riskantním situacím**: Zejména když ti zbývá poslední život

## Technické informace
- Plugin je implementován pomocí Skriptu
- Životy jsou ukládány do persistentní paměti a zachovávají se mezi restarty serveru
- Automatická synchronizace TAB menu každých 5 minut

---

Nyní si můžeš užít větší výzvu na serveru! Každý život se počítá, tak hraj opatrně a strategicky.