# Potok-inátor

**Odhadněte potenciál vašeho potoka pro výrobu elektrické energie.**

Potok-inátor je webová kalkulačka pro předběžný odhad výkonu malé vodní elektrárny využívající šroubovou turbínu (Archimédův šroub). Aplikace vás provede měřením základních parametrů potoka a vypočítá odhadovaný výkon v kilowattech.

## ⚠️ Upozornění

Tato aplikace je určena **pouze pro předběžný, hrubý odhad** a neměla by být používána pro žádný skutečný stavební projekt. Aplikace neposkytuje žádné informace týkající se technické ani právní proveditelnosti vašeho projektu. Vývojáři aplikace nepřebírají žádnou odpovědnost za jakékoli výpočty ani prohlášení učiněná na základě této aplikace.

## Funkce

Aplikace obsahuje 4 kroky měření:

1. **Odhad výšky pádu** - Měření nadmořské výšky na vstupu a výstupu potoka
2. **Odhad průřezu** - Měření průřezu koryta potoka (cirkusová metoda)
3. **Odhad rychlosti** - Měření rychlosti toku pomocí mostu a plovoucího objektu
4. **Účinnost** - Výpočet s použitím účinnosti šroubové turbíny (69%)

Aplikace obsahuje:
- ✅ Interaktivní vizualizace pro každý krok
- ✅ Průběžnou validaci vstupů
- ✅ Detailní vysvětlení výpočtu
- ✅ Responzivní design pro mobilní zařízení

## Jak používat

Aplikace je čistě HTML/JavaScript aplikace bez závislostí. Stačí otevřít [index.html](index.html) v moderním prohlížeči.

### Lokální spuštění

```bash
# Jednoduchý HTTP server
python -m http.server 8000
# nebo
npx serve
```

Pak otevřete prohlížeč na `http://localhost:8000`

## Technologie

- HTML5
- Tailwind CSS (CDN)
- Vanilla JavaScript
- SVG vizualizace

## Výpočetní vzorec

```
P (kW) = h × S × v × η × ρ × g / 1000
```

Kde:
- `h` = výška pádu (m)
- `S` = průměrný průřez (m²)
- `v` = rychlost toku (m/s)
- `η` = účinnost turbíny (0,69)
- `ρ` = hustota vody (1000 kg/m³)
- `g` = tíhové zrychlení (9,81 m/s²)

## Autoři

- **Výpočty a metodologie:** Julia Tanzer
- **Vytvoření aplikace:** Jan Odstrčilík (pomocí AI)

## Licence

Tato aplikace je poskytována "jak je" bez jakýchkoli záruk.
