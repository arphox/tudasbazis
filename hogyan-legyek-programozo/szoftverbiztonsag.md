# Szoftverbiztonság
Szoftverrendszerek esetén az adott rendszer felhasználási céljától függően kisebb-nagyobb figyelmet kell arra szentelni,
hogy a rendszer biztonságos legyen.

Itt a használt technológiától függően ezernyi témát meg lehetne említeni, de megpróbáltuk összeszedni azokat az elveket,
amelyeket talán minden programozónak ismernie kell.

## Általános elvek
- [jelszótárolás módjai](https://www.refaktor.hu/biztonsagos-jelszotarolas/)
- hashelés, néhány hash algoritmust meg tudj említeni (MD5, SHA, bcrypt)
- "sózás" (kriptográfiai értelemben)
- titkosítás, néhány algoritmus említés szintjén (RSA, AES, Blowfish, Twofish)

## Adatbázis-védelem
- SQL injekció megértése, kivédésének lehetőségei
- webszerveren tetszőleges fájlok elérésének megakadályozása

## Behatolásvédelem (natív programok esetén)
**Ha** nem menedzselt nyelvet használsz (pl. C-t), érdekesek lehetnek az alábbiak is:
- puffertúlcsordulás veszélyei
- egész számok túlcsordulásának a veszélyei
- exploitok
- shellcode
- ROP lánc

---------------------------
## Haladó rész

### Gyakori hibák
A Top 10 kihasználható hibákról az OWASP oldalán tudsz olvasni (angolul) [itt](https://www.owasp.org/index.php/OWASP_Top_Ten_Cheat_Sheet).

### Gyakorlás
Ha szeretnél látni és gyakorolni olyan programokon amik tanítási célzatból úgy lettek megírva, hogy hibásak legyenek, akkor ajánlottak:
- [DVWA](http://www.dvwa.co.uk/) (Web)
- [DIVA](https://github.com/payatu/diva-android) (Android)

### Biztonsági ellenőrző listák 

- [Security Checklist (általános informatikai)](https://securitycheckli.st/)
- [PHP](https://hackernoon.com/the-ultimate-php-security-checklist-eec9895f2fa3) _angol_
- [Node.JS](https://medium.com/@nodepractices/were-under-attack-23-node-js-security-best-practices-e33c146cb87d) _angol_
