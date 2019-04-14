# Szoftverbiztonság
Szoftverrendszerek esetén az adott rendszer felhasználási céljától függően kisebb-nagyobb figyelmet kell arra szentelni,
hogy a rendszer biztonságos legyen.

Itt a használt technológiától függően ezernyi témát meg lehetne említeni, de megpróbáltuk összeszedni azokat az elveket,
amelyeket talán minden programozónak ismernie kell.

## Általános elvek
- jelszótárolás módjai ("plain text" soha!)
- hashelés, néhány hash algoritmust meg tudj említeni (MD5, SHA, bcrypt)
- "sózás" (kriptográfiai értelemben)
- titkosítás, néhány algoritmus említés szintjén (RSA, AES, Blowfish, Twofish)

## Adatbázis-védelem
- SQL injekció megértése, kivédésének lehetőségei
- webszerveren tetszőleges fájlok elérésének megakadályozása

----------------------------------------------------------------
### Behatolásvédelem (natív programok esetén)
**Ha** nem menedzselt nyelvet használsz (pl. C-t), érdekesek lehetnek az alábbiak is:
- puffertúlcsordulás veszélyei
- egész számok túlcsordulásának a veszélyei
- exploitok
- shellcode
- ROP lánc
