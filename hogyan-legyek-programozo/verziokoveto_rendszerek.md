# Verziókövető rendszerek

## Bevezető

Gondoljunk bele néhány dologba:
1. A legtöbb projektet nem egy ember visz véghez, ami azt jelenti, hogy valahogy forráskód-szinten is menedzselni kellene a közös munkát. Talán zip fájlok oda-vissza küldözgetése nem a legjobb mód erre.
2. Időnként szükség lehet a forráskód egy előző állapotára visszaállni; mert elrontottunk valamit, vagy mert kíváncsi vagyunk, hogy valami régebben hogy volt.
3. A kódon történő változásokat hasznos lenne "kötegekbe" foglalni, aminek külön nevet és leírást lehetne adni. Így nagyjából átlátnánk, hogy egy "köteg" mit változtatott a kódon.

A verziókövető rendszerek ezeket a feladatokat igyekeznek megoldani.

Néhány leírás a verziókövető rendszerekről, olvasgatni:
- [Atlassian](https://www.atlassian.com/git/tutorials/what-is-version-control)
- [git-scm](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control).

Szinte minden valamire való vállalatnál a forráskódot verziókövető rendszerekben tárolják.
> _Jó tanács_: olyan céghez ne menj programozónak, ahol nem használnak semmilyen verziókövető rendszert.

## Osztályozásuk

### Centralizált (központosított) verziókövető rendszerek
A centralizált rendszerek egy vagy több központi helyen tárolják az információt.
Az ilyen rendszerek esetén a kliens gépen a forráskód mindig csak egy aktuális állapota látható (általában a legfrissebb).

Előnyei:
- könnyen érthető modell
- jobb jogosultságkezelés: a kód különböző részeihez különböző jogosultsági szinteket lehet rendelni
- könnyebben átlátható, hogy a kód bizonyos részein ki dolgozik, ugyanis mindenki szinkronban van a szerverrel

Hátrányai:
- minden a központi szerveren van; ha arról elveszik az adat, minden elveszik
- ha a központi szerverrel nincs kapcsolat, a munka nehézkessé válhat

Példák ilyen rendszerekre:
- TFS (Team Foundation Server)
- Subversion
- Perforce

### Elosztott verziókövető rendszerek
A forráskód teljes állapota annak "történelmével" együtt több példányban megtalálható a különböző klienseknél.
A szerver léte itt nem kötelező, de a gyakorlatban az egyszerű kezelhetőség érdekében szinte mindig van.
Az open-source világ nagy része elosztott verziókövetőrendszereket használ, főként git-et.

Előnyei:
- nem szükséges állandó hálózati kapcsolat
- a branch-elés egyszerű, gyors, és "lightweight" (nem igényel duplikált adattárolást)
- általában gyorsabban működik, révén nem egy központi szerveren történik minden hanem lokálisan

Hátrányai:
- kissé körülményesebb őket használni, mint a centralizált rendszereket
- "a forráskód egész történelme" esetenként nagyra hízhat (leginkább akkor, ha rosszul használják, pl. nagy méretű fájlokat tartanak source control alatt)
- a jogosultságkezelés nehezen megoldható, révén a forráskód egésze mindenkinél megtalálható

> _Megjegyzés:_ ilyen rendszereknél a jogosultságkezelés problémáján segíthet az, ha a szoftver részekre van tagolva,
és a különböző részek különböző repository-kban találhatóak meg, így azokhoz különböző jogosultságok rendelhetőek (repository-szintű jogosultságok léteznek).

Példák ilyen rendszerekre:
- Git
- Mercurial

## Git
A gitre azért szentelünk egy külön fejezetet, mert jelenleg ez a legismertebb verziókezelő rendszer, 
és minden fejlesztőnek illik ismernie.

Linkek a git elsajátításhoz:
- [Atlassian](https://www.atlassian.com/git/tutorials): rengeteg, jó leírás a gitről általánosságban.
- [git - the simple guide](http://rogerdudler.github.io/git-guide/): egyszerű, "színes" leírás a gitről. Jó kiegészítő/ismétlő egy részletesebb guide elolvasása után.
- [GitHub Git Handbook](https://guides.github.com/introduction/git-handbook/): viszonylag rövid leírás a gitről, a GitHub-tól.
- [Github Try](https://try.github.io)
- [Learn Git Branching](https://learngitbranching.js.org)
