# VWAP Divergence

A **VWAP Divergence** indikátor célja, hogy segítsen felismerni a lehetséges fordulópontokat a piacon azzal, hogy a kereskedési volumen súlyozott átlagárának (VWAP) mozgását összehasonlítja az aktuális árfolyam változásával. Amikor ez a két érték - a VWAP és a piaci ár - ellentétes irányba mozdul el, azt divergenciának nevezzük. Ez lehet bullish (potenciális áremelkedésre utaló) vagy bearish (potenciális árcsökkenésre utaló) jelzés.

## Miért hasznos a VWAP Divergence indikátor?
1. **Pontosan mutatja a volumen hatását**

    A VWAP (Volume Weighted Average Price) nem egyszerű mozgóátlag, hanem a kereskedett volumen is befolyásolja. Így reálisabban tükrözi a piaci helyzetet, mint egy pusztán ár-alapú mutató.

2. **Divergencia = Fordulópont?**

    Ha az ár emelkedik, de a VWAP inkább csökken (vagy nem követi az áremelkedés ütemét), az bullish divergenciát jelezhet – a „nagyobb játékosok” (akik a volument adják) lehet, hogy még nem kezdték meg a felvásárlást, de hamarosan követhetik a trendet. Fordítva pedig, ha az ár csökken és a VWAP emelkedik, az bearish divergenciára utalhat – a piacban erős eladói nyomás jöhet.

3. **Kereskedési döntések kiegészítője**

    A divergenciák nem garantálják a fordulatot, de sok kereskedő hasznosnak találja, ha más eszközökkel (pl. támasz-ellenállás szintek, RSI, MACD, gyertyaformációk stb.) együtt elemzi őket. A divergens mozgások gyakran jelzik egy trend kifulladását vagy megfordulását.

## Hogyan értelmezzük a jelzéseket?
- **Bullish Divergence**
    
    Általában akkor jelentkezik, ha az árak elkezdenek felfelé mozogni, de a VWAP (volumensúlyozott átlag) még nem követi az emelkedést, vagy lefelé tart. Ez arra utalhat, hogy a „nagypénz” vagy a fő piaci szereplők egyelőre óvatosak, de a későbbiekben bekapcsolódhatnak a vásárlásba, ami további áremelkedést eredményezhet.

    - A grafikonon zöld színnel, a gyertya alatt jeleníti meg a script.

- **Bearish Divergence**

    Akkor alakul ki, ha az árak eső tendenciát mutatnak, miközben a VWAP még emelkedik. Ez arra utalhat, hogy a piac elkezdett gyengülni, és a „nagypénz” szereplők egyre inkább feladják a long pozíciókat vagy elkezdenek short pozíciókat nyitni.

    - A grafikonon piros színnel, a gyertya fölött jelzi a script.


## Mikor lehet különösen hasznos?
- **Volumenerős piaci helyzetekben**

    Mivel a VWAP a volumennel súlyoz, különösen az erős forgalmú, likvid piacokon (pl. devizapiac, nagyobb részvények, kriptók) adhat valós képet.

- **Kulcsfontosságú technikai szinteknél**

    Például támasz, ellenállás vagy Fibonacci-szintek közelében a divergencia megerősítheti a forgatókönyvet, hogy a piac fordulatot vehet.

- **Stratégiák kiegészítéseként**

    A divergenciajelzés önmagában nem feltétlenül elég. Érdemes más indikátorokkal, illetve saját kereskedési szabályrendszerrel (stop-loss, célárak stb.) együtt használni.

## Előnyök és korlátok

### Előnyök

- A divergens mozgások korai jelzést adhatnak a lehetséges trendváltásról.
- A VWAP a volumenen alapul, így a nagybefektetők mozgásait is segíthet észlelni.

### Korlátok

- Nem garantálja a fordulatot; bizonyos divergenciák „hamis” szignált is adhatnak.
- Alacsony forgalmú instrumentumoknál a VWAP kevésbé lehet megbízható.
- Mindig érdemes megerősítést kérni más indikátoroktól vagy a piaci struktúrától.

## Gyakorlati Tippek

1. **Több idősík összevetése**

    Vizsgáld az indikátor jelzéseit például 1 órás és napi grafikonon is. Ha mindkettőn hasonló divergenciát látsz, az erősebb jelzés lehet.

2. **Ne hagyd figyelmen kívül a volatilitást!**
    
    A script ATR-rel (Average True Range) dolgozik, így ha extrém volatilitás vagy éppen nagyon alacsony volatilitás jellemző a piacra, érdemes lehet módosítani az ATR-szorzót (pl. 2x, 3x).

3. **Stop-loss és kockázatkezelés**

    Mint minden kereskedési jelzésnél, itt is kulcsfontosságú, hogy előre meghatározd, hol lépsz ki, ha a piac nem abba az irányba mozog, ahogy vártad.

4. **Fontos Figyelmeztetés**

    Ez az indikátor nem helyettesíti a saját elemzést, és nem garantálja a profitszerzést. A múltbeli mintázatok nem biztos, hogy a jövőben is ugyanúgy működnek. Mindig győződj meg róla, hogy megérted a kockázatokat, és felelősségteljesen kezeld a kereskedési döntéseidet.