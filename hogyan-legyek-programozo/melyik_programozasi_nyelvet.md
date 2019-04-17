# Melyik programozási nyelvet válasszam?
## Kezdőknek ajánlott programozási nyelvek
Van egy színes-szagos [kép](https://raw.githubusercontent.com/arphox/tudasbazis/melyik_programozasi_nyelvet/kepek/melyik_programozasi_nyelvet.png) az interneten, amelyet érdemes átfutni, habár fenntartásokkal kell kezelni, helyenként elfogult lehet.

> Fontos, hogy a következő nyelveket **első nyelvnek** ajánljuk. Rengeteg kiváló haladó nyelv van, amelyeket szívesen felírtunk volna a listára, de egy programozást most tanuló **kezdő** számára nem igazán megfelelőek.

Először leginkább azt kell eldöntened, hogy milyen területre szeretnél programozni.

### 1. Webprogramozás
Manapság ez a legnagyobb területe a programozásnak, ezt a [2019-es SOF Dev Survey](https://insights.stackoverflow.com/survey/2019#developer-roles) is alátámasztja.
- **Nyelvek**:
  - Frontend: HTML **és** CSS **és** JavaScript (mindhárom szükséges; az első kettő jelölőnyelv, a harmadik programozási nyelv)
    - [TypeScript](https://github.com/Microsoft/TypeScript)
  - Backend: JavaScript (Node.js), PHP, Java, C#, ASP.NET MVC

### 2. Beágyazott rendszerek programozása
Ha beágyazott hardverre szeretnél programot írni, alacsonyabb szintre kell menned.
Itt egyértelműen C-vel érdemes kezdeni, ott értheted meg csak igazán a beágyazott rendszerek lelki világát, de ha egy kicsit könnyebb és kezdő-barátibb szeretnél, akkor érdemes az arduinoval kezdeni. Ezt programozhatod már c és c++ nyelven is és nagyon sok előre megírt könyvtár van hozzá. Szintúgy nagyon sok előre elkésíztett hardveres modul van a motorokon, szivattyúkon, hőmérőkön keresztül egészen a különböző relékig. Ehhez kapcsolódó, illetve ritkén, de használható nyelvek: Java, Python, Rust, Javascript, LUA; vagy ha nagyon alacsony szinten kezdenél (segítség és előismeretek nélkül nem ajánlott): Assembly

Munkában ha iylen területről van szó, akkor a legtöbb helyen C nyelvet használnak, így a fent sorolt alternatívák javarészt hobbira, vagy néhány ritka esetre használatosak.

### 3. Mobilalkalmazások programozás
Platformtól függően (leggyakrabban):
- Android: **Java**
- iOS: **Swift**

Még több választási lehetőség: Kotlin, C++, C#, JavaScript, Python

Ezeken kívül van több univerzális fejlesztőkörnyezet ami a megírt kódunkat több eszközre is le tudja fordítani egyszerre (például Android és iOS). Ilyenek többek között a:
- Xamarin
- Unity

### 4. Asztali alkalmazások (általános célú nyelvek)
Ha nem tudod még, hogy mivel akarsz foglalkozni, csak "simán" meg akarsz tanulni programozni, az alábbi a nyelveket ajánljuk.
Ha aszerint szeretnél választani, hogy melyik nyelvvel lehet jelenleg a legtöbbet keresni a piacon, akkor [itt](https://insights.stackoverflow.com/survey/2019#top-paying-technologies) nézelődj, [itt](https://insights.stackoverflow.com/survey/2019#most-popular-technologies) pedig a legnépszerűbb nyelveket találod.

Tehát az ajánlott általános nyelvek kezdőknek:
- Python
- JavaScript
- Java
- C#

-----------------------------------------------------------
Érdemes átolvasni azt is, hogy hogyan csoportosíthatjuk a nyelveket.
Kezdőként nem valószínű, hogy ezt át fogod látni, de legalább egyszer olvastál róla, és legfeljebb később visszatérsz ide valami kapcsán.

## Csoportosítás
Fontos megjegyezni, hogy sok programozási nyelv nem illeszthető be egy kategóriába, ugyanis általános célú programozási nyelvnek tekinthetőek.
Ezekre néhány példa: JavaScript, Python, Java, C#, PHP, C++, TypeScript, C, Ruby, Go, stb.

> A csoportosítás ismerete nem fontos egy kezdő számára, de egyszer mindenképpen olvasd el, hogy legalább tudj róluk.

### 1. Imperatív nyelvek
Imperatív nyelvek esetén a programnak azt adod meg, hogy egy feladatot _hogyan_ oldjon meg.
- Procedurális nyelvek: C, Pascal
- Objektumorientált nyelvek: C++, C#, Java

### 2. Deklaratív nyelvek
Az imperatív nyelvekkel ellentétben itt azt fogalmazod meg, hogy _mit_ szeretnél, hogy megoldjon a program; a _hogyan_-t pedig rábízod.
- Funkcionális nyelvek: Haskell, Erlang, ML (Meta Language), F#, Lisp
- Logikai nyelvek: Prolog

### Típusosság ideje
Típusosság szerint lehet egy nyelv **statikusan**, vagy **dinamikusan** típusos.
- A statikusan típusos nyelveken írt programokat a futtatás előtt, tipikusan egy fordító (compiler) ellenőrzi. Példák: C, C++, Java
- A dinamikusan típusos nyelveken írt programok típusellenőrzése a futásidőben történik: Python, Ruby, JavaScript

### Típusosság erőssége
Ez leginkább azt mutatja meg, hogy a nyelv mennyire kezeli "lazán" a típusokat.
- erősen típusos nyelvek, pl. Java, C#
- gyengén típusos nyelvek, pl. PHP, JavaScript

### Memóriamenedzsment szempontjából
- **Natív/nem menedzselt (unmanaged) programozási nyelvek**:
Ezek segítségével közvetlenül a számítógép által végrehajtható kódot kapsz. Ezek neves képviselője a C és C++.
Ha natívan programozol, teljes kontrollod van szinte minden felett. Viszont ha natívan programozik az ember, akkor sok dologra oda kell figyelni, és ha elrontod, akkor máris hátsóajtót nyithatsz mindenféle kártevő programnak.

- **Menedzselt (managed) programozási nyelvek**:
Ezek során a programot egy másik program, az ún. futtató környezet fogja végrehajtani.
Ennek a csoportnak képviselői a manapság használatos legtöbb nyelv: C#, Java, PHP, JavaScript, Python, Perl, stb.
Ezeknél valamivel kevesebb ráhatásod van arra, hogy mi történik a háttérben és biztonsági rések miatt is kevesebbet kell aggódnod.
Viszont, biztonsági rés még mindig lehet a futtatókörnyezetben, és te nem igazán tehetsz ellene semmit, amíg a futtató környezet fejlesztői ki nem javítják azt.
De ezek miatt általában nem kell aggódni.

### Implementáció szempontjából
Egy programozási nyelv [implementációja](https://en.wikipedia.org/wiki/Programming_language_implementation) annak futtatási módját határozza meg.
Ehhez két megközelítést alkalmaznak, habár a hibrid megoldások (JIT/AOT compilerek) is gyakoriak:
- fordítás ("compiler"): a forráskódot a compiler lefordítja egy másik kódra, amit majd a következő réteg majd fordít/interpretál.
- interpretálás ("interpreter"): a forráskódot közvetlenül, utasításonként (vagy tetszőleges blokkonként) értelmezi és azonnal futtatja.

> _Érdekesség_: a legalacsonyabb, még nem elektronikai szinten azaz a processzor mikroarchitektúrájának szintjén interpretálás zajlik: a processzor folyamatosan kapja az utasításokat majd azonnal végrehajtja őket.


----------------------------------------------------
- **Megjegyzések**:
A következő forrásokat használtuk fel: [Google](https://www.google.com/), [Stack Overflow Developer Survey Results 2019](https://insights.stackoverflow.com/survey/2019), [TIOBE Index](https://www.tiobe.com/tiobe-index/), [PYPL](http://pypl.github.io/PYPL.html)
