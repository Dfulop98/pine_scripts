# Fibonacci Golden Wave – Alapvető háttér és koncepció

A Fibonacci Golden Wave elnevezés mögött elsősorban a Fibonacci-szintek és a hozzájuk kapcsolódó „aranymetszés” (golden ratio) gondolata áll.A kereskedésben és a technikai elemzésben a Fibonacci-számok és az aranymetszés azon az elven alapulnak, hogy a természetben (beleértve a piaci mozgásokat is) gyakran megfigyelhető bizonyos ismétlődő arányosság vagy struktúra. Ezeket az arányokat (például 0,236; 0,382; 0,5; 0,618; 0,786) a Fibonacci-szintek határozzák meg, amelyeket sok kereskedő támasz- vagy ellenállás-szintként figyel a piacokon.


## 1. A Fibonacci-szintek és az aranymetszés jelentősége

#### Fibonacci-számok

- A Fibonacci-sorozat 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55 stb. elemekből áll, ahol minden új elem az előző két elem összege.
- A technikai elemzésben ugyan nem közvetlenül magukat a Fibonacci-számokat, hanem az ezekből levezetett arányokat (0,236; 0,382; 0,5; 0,618; 0,786 stb.) használjuk szintek meghatározására.

#### Aranymetszés (golden ratio)

- Az aranymetszés általában a `𝜙 = 1,618...` és az `1 / 𝜙 ≈ 0,618` értékkel hozható összefüggésbe.
- Ez az aránypár a természetben és a művészetekben is kiemelten gyakran előforduló „harmonikus” viszony.
- A piaci elemzésben a 0,618 (vagy 61,8%) szint különösen fontos, mert sokszor ehhez kötik a korrekciók során kialakuló lehetséges fordulópontokat.


## 2. Hogyan kapcsolódik ez a kereskedéshez?

- **Retracementek (visszahúzódások):** Amikor az árfolyam egy nagyobb trendmozgás után elkezd korrigálni, a korrekció vége gyakran (de nem törvényszerűen!) a fontos Fibonacci-szintek környékén alakul ki.

- **Támasz és ellenállás:** A Fibonacci-szintek – különösen a 0,382; 0,5; 0,618 – gyakran szolgálnak olyan szintekként, ahol megnövekszik a piaci aktivitás, mert sok kereskedő figyeli ezeket a pontokat.

- **„Golden Zone”:** Sokan a 0,5 és 0,618 közötti sávot nevezik „arany zónának”, mert a tapasztalatok szerint viszonylag gyakran itt fejeződik be egy visszahúzódás, és fordulhat vissza az árfolyam a korábbi trend irányába.


## 3. A script fő logikája (röviden, kód nélkül)

- **Pivots (local high/low) azonosítása**

    Először felismerjük a helyi csúcsokat (pivot high) és mélypontokat (pivot low), vagy manuálisan (az elmúlt N gyertya legmagasabb/alacsonyabb pontját figyelve), vagy a Pine Script beépített ta.> pivothigh / ta.pivotlow függvényeivel.

- **Legutóbbi csúcs és völgy kijelölése**

    Legutolsó csúcsot és völgyet használjuk alapul a Fibonacci-számításokhoz (például a legutóbbi pivot high árfolyama lehet a maximum, a legutóbbi pivot low ára pedig a minimum).

- **Fibonacci-szintek kiszámítása**

    - A különbség (legutóbbi csúcs − legutóbbi völgy) szorozva a kiválasztott Fibonacci-arányokkal (pl. 0,5 és 0,618) adja azt a visszahúzódást, ami alapján megrajzolja a két szintet.

    - A megjelenített sáv (Golden Zone) vizuálisan segít a kereskedőnek eldönteni, hol lehet a korrekció vége.

- **Vizuális jelzések**
    A script vonalakkal és (opcionálisan) kitöltött zónával mutatja meg a Fibonacci-árszinteket, így kiemeli a potenciális korrekciós területet.


## 4. Miért lehet hasznos?
- **Támogatás/Ellenállás:** A kereskedők a Fibonacci-szinteket gyakran kritikus támasz- vagy ellenállás-szintként használják, ahol a piac gyakran fordul.

- **Stop/Target meghatározás:** Könnyebb lehet a stop loss vagy a profitcél szintjeit kijelölni, ha tudjuk, hol várható jelentős árfolyamreakció.

- **Trendfolytatás valószínűsége:** Ha a korrekció éppen az arany zónáig jut, és onnan fordul, sokan ebből arra következtetnek, hogy a nagyobb trend folytatódik.

## 5. Mire figyeljünk?
- **Nem garancia:** Mint minden indikátor vagy eszköz a technikai elemzésben, a Fibonacci Golden Wave sem garantál biztos belépési vagy kilépési pontot; csupán támpontot ad.

- **Egyéb megerősítés:** Érdemes más elemzési módszerekkel (pl. volumen, trendvonalak, gyertyaalakzatok) kiegészíteni, hogy megbízhatóbb képet kapjunk.

- **Időkeret:** Különböző időtávokon a Fibonacci-szintek is más és más értéket vehetnek fel. Nagyobb idősíkon (pl. napi, heti) erősebbnek tartják, de rövidebb idősíkon (pl. 15 perces) is sokan alkalmazzák a napi kereskedésben.

## 6. Összefoglalás

A Fibonacci Golden Wave lényegében a legutóbbi piaci mozgás csúcs- és völgyértékei között meghatározott Fibonacci-visszahúzódási zónákra épül. A kereskedők gyakran követik ezeket az arányszámokat (különös tekintettel a 61,8%-ra és a 50%-ra), mivel ezek körül gyakran megnő a vételi vagy eladási aktivitás. A script célja, hogy automatikusan felismerje a releváns csúcsokat és mélypontokat, majd megjelenítse a legfontosabb Fibonacci-szinteket, segítve ezzel a felhasználókat a potenciális piaci fordulópontok azonosításában.

Ez a módszer a technikai elemzés egyik hasznos, de nem kizárólagos eleme: más eszközökkel együtt alkalmazva jelenthet nagyobb megbízhatóságot a piaci döntéshozatalban.