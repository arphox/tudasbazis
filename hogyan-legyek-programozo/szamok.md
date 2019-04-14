# Számok

Mivel minden számítógépes program számokkal dolgozik, érdemes megérteni, hogy ez _legalább nagy vonalakban_ hogyan történik.

## Számrendszerek, számábrázolás
A számítógépek túlnyomó része **nem** tízes, hanem kettes (bináris) számrendszerben dolgozik; ezért érdemes az utóbbit megismerni ha még nem ismered.

> **Megjegyzés**: a fejlesztők mindennapi munkája során ritkán van szükség bináris számokkal való számolásra, kézzel.
Azonban időnként előfordulhatnak olyan esetek, amikor erre a tudásra közvetett módon szükség van.

### Bináris (kettes) számrendszer

Ide tartozó témakörök, címszavakban:
- bináris számrendszer
- bit és bájt, [SI-prefixumok](https://hu.wikipedia.org/wiki/SI-prefixum)
- [bináris prefixum](https://hu.wikipedia.org/wiki/Bin%C3%A1ris_prefixum): "megabájt(MB) vs. mebibájt(MiB)?"
- bináris egész számok ábrázolása
- kettes komplemens számábrázolás
- 8, 16, 32 és 64 bites egész számok értelmezési tartománya
- lebegőpontos számábrázolás
- IEEE lebegőpontos számformátum (szabvány)
- NaN, végtelen és 0 ábrázolása lebegőpontosan

### Hexadecimális (tizenhatos) számrendszer
- a hexadecimális számrendszer jelentősége
- a hexadecimális számrendszer összevetése a bináris számrendszerrel, átváltás a kettő között

## Műveletek számokkal
A számokat nem csak ábrázolni kell, hanem számolni is kell velük.
A számítógép nem ér sokat, hogyha nem számolsz vele.
Bármilyen programozási nyelvet tanulsz, előbb vagy utóbb számolnod kell, és meg kell értened, hogy egyes számítási módoknak melyek az előnyei, hátrányai és határai.

**Címszavak**:
- a 4 aritmetikai alapművelet (+, -, *, /)
- milyen gyorsan hajtódnak ezek végre, melyiket a leggyorsabb és melyiket a leglassabb végrehajtani?
- maradékképzés
- túlcsordulás megértése
- lebegőpontos számok pontossága és hibái
- hogyan hasonlítasz össze két lebegőpontos számot, hogy egyenlőek-e?

## Logikai műveletek
- logikai műveletek: nem (`NOT`), vagy (`OR`), és (`AND`), kizáró vagy (`XOR`)
- [De Morgan-azonosságok](https://hu.wikipedia.org/wiki/De_Morgan-azonoss%C3%A1gok)
- bitszintű logikai műveletek

## Gyakorlati jelentőségű témák
- hogyan állíthatunk 1-esre vagy 0-ra biteket egy tetszőleges számban?
- [maszkolás](https://en.wikipedia.org/wiki/Mask_(computing))
- eltolások (shifting): balra tolás, jobbra tolás, előjeles jobbra tolás
    - milyen kapcsolatban van ez a kettő hatványaival történő szorzással, osztással?

----------------------------------------------------------

### Extra - kapcsolódó poénok
Amelyeket a téma ismerői már megértenek:

**A programozó és a felesége**
- `Feleség`: Drágám, szaladj le a közértbe, hozz egy doboz tejet és ha van tojás, hozz hatot!
- _A programozó lemegy a boltba, vesz hat doboz tejet, majd hazamegy._
- `Feleség`: Mi a francért vettél hat doboz tejet?
- `Programozó`: Volt tojás!

**Miért keverik össze a programozók a Halloweent a Karácsonnyal?**
- Mert nekik az `OCT 31` ugyanaz, mint `DEC 25`!
