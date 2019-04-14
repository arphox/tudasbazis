# Adatbázisok
## Bevezető
A legtöbb szoftverprojektben használnak adatbázisokat, így egy fejlesztőnek érdemes tudnia többet-keveset (attól függően, hogy hol dolgozik) róluk.
_"Az adatbázisok célja adatok megbízható, hosszú távon tartós ("perzisztens") tárolása, és viszonylag gyors visszakereshetőségének biztosítása."_[[1]](https://hu.wikipedia.org/wiki/Adatb%C3%A1zis)


Ha abból a fogalomból indulunk ki, hogy az adatbázis _"adatok szervezett/strukturált elektronikus gyűjteménye"_ [[2]](https://en.wikipedia.org/wiki/Database),
akkor már egy egyszerű szöveges fájl (txt) is adatbázisnak tekinthető, ám a köztudatban adatbázis alatt inkább az erre a célra kialakított külön rendszereket/szoftvercsomagokat értjük.

## Címszavak
Minden részletre kiterjedt csoportosítások helyett áttekintendő címszavak:
- adatbázis
- adatbázis modell (többféle gondolkodásmód, ahogyan az adatokat tárolják, [pl.](https://en.wikipedia.org/wiki/Database_model))
- SQL: érdemes egyszer részletesen áttanulmányozni ezt a nyelvet; relációs adatbázisokban, így sok munkahelyen is szükség lehet rá
- "in-memory" adatbázis
- cloud adatbázis
- [adatbázis-motorok rangsorolása](https://db-engines.com/en/ranking)

Alapvetően tanácsolható, hogy nézz meg minden népszerű modellből legalább egy rendszert:
- relációs: Oracle, MySQL, Microsoft SQL Server, PostgreSQL
- "kulcs-érték"(key-value): **Redis**, Amazon DynamoDB, Memcached, Microsoft Azure Cosmos DB
- dokumentum alapú: **MongoDB**, Amazon DynamoDB
- keresőmotor: Elasticsearch, Splunk, Solr

> Az adott modellen belül a sorrend népszerűséget jelöl, és [innen](https://db-engines.com/en/ranking) származik.
