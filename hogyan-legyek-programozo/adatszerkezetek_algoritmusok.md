# Adatszerkezetek, algoritmusok
A két témakör szorosan összefügg, hiszen egy algoritmushoz mindig szükség van valamilyen adatszerkezetre.

## Bevezető
Címszavak:
- adatszerkezet
- algoritmus

Alapvető algoritmusleíró elemek:
- értékadás
- elágazások (szelekció)
- ciklusok (iteráció)

Ezen kívül még olvass utána:
- alprogramok: függvény, eljárás, metódus

## Adatszerkezetek
### Egyszerű adatszerkezetek
Ismerd meg az általad választott programozási nyelv beépített, egyszerű típusait.

Íme néhány egyszerű adatszerkezet, amellyel sok nyelvben találkozhatsz:
- egész szám (integer, `int`)
- lebegőpontos szám (floating-point, `float`, `double`, stb.)
- karakter (character, `char`)
- logikai (boolean, `bool`)

### Összetett adatszerkezetek
Összetett adatszerkezetből rengeteg létezik. Egyeseket implementáltak az általad használt nyelven, egyeseket nem.

**Fontos**: a különböző adatszerkezetek különböző célokat szolgálnak. Vannak általánosabbak, mint például a tömb vagy a lista;
és vannak nagyon specializáltak.
Legtöbbször a gyakorlatban listát/tömböt használunk, de ettől függetlenül illik ismerni a többi alternatívát is.

Amiknek érdemes utána nézni:
- tömb (statikus, dinamikusan növekvő, rendezett, asszociatív)
- lista (tömb alapú, láncolt, [pl. itt](https://infoc.eet.bme.hu/ea10/))
- halmaz
- stack ("verem")
- queue ("sor")
- gráf, fa

Ezeket próbáld ki az általan választott nyelven, nézz utána hogy melyiknek mi az előnye és a hátránya.

## Algoritmusok
Az algoritmikus gondolkodás a programozói szakma egyik alapkövének tekinthető.
Röviden: aki nem tud így gondolkodni, minden bizonnyal csapnivaló programozó.

Kezdőként **nem** az a fontos, hogy bemagold az összes algoritmust, ami szembejön, hanem az, hogy _megértsd_ őket.
Az algoritmikus gondolkodásod fejlesztésére jó módszer a már létező algoritmusok megértése, kipróbálása a választott nyelveden.
Ez mondhatni "csak" a tanulási folyamat során kell; a mindennapi munkában leginkább mások által megírt algoritmusokat fogsz használni (a nyelvhez gyárilag adott algoritmusok formájában vagy külső osztálykönyvtárakból).

> _Megjegyzés_: A kódújrafelhasználás a modern programozás fontos része: ha mindig mindenki újból "feltalálta volna a kereket", sehol sem tartanánk az informatikával.

### Programozási "tételek"
Érdemes ezeket részletekbe menően megérteni.

**Egyszerű programozási tételek**:
- sorozatszámítás
- eldöntés
- kiválasztás
- lineáris keresés
- bináris keresés
- megszámolás
- maximumkiválasztás

**Összetett programozási tételek:**
- másolás
- kiválogatás
- szétválogatás
- metszet
- egyesítés
- összefuttatás

### Rendező algoritmusok
Tanulmányozásukat leginkább az algoritmikus gondolkodás javítására ajánljuk, hiszen a mindennapi munka során valószínűleg egy beépített rendező algoritmust fogunk használni.

Jó sok olvasnivaló erről [itt](https://en.wikipedia.org/wiki/Sorting_algorithm).

"Kisiskolás" rendező algoritmusok:
- egyszerű cserés rendezés
- minimumkiválasztásos rendezés (minimum selection sort)
- buborékos rendezés (bubble sort)
- beillesztéses rendezés (insertion sort)

Haladó algoritmusok:
- merge sort
- quicksort

Egyéb algoritmusok (nem összehasonlítás-alapon működnek):
- Pigeonhole sort
- Counting sort
- Radix Sort

### Rekurzív algoritmusok
A rekurziós algoritmusok másfajta gondolkodást igényelnek, ezért érdemes ezeket megismerni.
Erről jó sok leírás [itt](https://en.wikipedia.org/wiki/Recursion_(computer_science)).

Néhány példafeladat erre:
- faktoriális
- legnagyobb közös osztó
- Hanoi tornyai

### Egyéb
- futási idő komplexitás ([pl.](https://ithub.hu/blog/post/Amit_tudnod_kell_fejlesztokent_II_resz_Algoritmusok_es_komplexitas/))
- [fabejáró algoritmusok](https://en.wikipedia.org/wiki/Tree_traversal)
- gráfalgoritmusok

-------------------------------------------------
Források:
- [ELTE IK Programozási Alapismeretek](http://progalap.elte.hu/downloads/seged/eTananyag/)
