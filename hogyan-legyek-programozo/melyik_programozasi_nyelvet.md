# Milyen programozási nyelvet válasszak?
Mielőtt megnéznénk a választási lehetőségeket, nézzük meg azt, hogy hogyan csoportosítjuk a programozási nyelveket.

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

----------------------------------------------------

## Kezdőknek ajánlott programozási nyelvek
Van egy ilyen kép az interneten

> Fontos, hogy a következő nyelvek között semmilyen sorrendiség nem áll fent. A szöveg jellege miatt nem tudjuk őket egymás mellett ábrázolni, csak egymás alatt; így mindenképpen az egyiknek elsőnek kell lennie.
