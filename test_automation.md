# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

## A tesztelés alapjai:
#### Mi a tesztelés célja? Mi nem az?
Célja: hibák feltárása, kockázatok csökkentése, minőség biztosítása, annak ellenőrzése, hogy a rendszer megfelel a követelményeknek.
Nem célja: a hibák teljes hiányának bizonyítása. Teszteléssel nem lehet 100%-ban bizonyítani, hogy nincs hiba a rendszerben.
#### Mi a kapcsolat a tesztelés és a hibamegelőzés között?
A tesztelés nem csak hibák keresése, hanem hibamegelőző eszköz is: ha korai fázisban tesztelünk (pl. követelmények felülvizsgálata), akkor sok hiba megelőzhető, mielőtt bekerülne a kódba.
#### Miért fontos, hogy a tesztelők függetlenek legyenek a fejlesztőktől?
Objektív hibakeresés: a fejlesztő elfogult lehet a saját kódjával szemben, kevésbé veszi észre a hibát.
Friss szemmel könnyebb észrevenni a problémákat.
#### Mi a veszélye annak, ha a fejlesztő maga teszteli a saját kódját?
Nem biztos, hogy észreveszi a saját hibáit, mert „úgy gondolkodik, mint a fejlesztő”.
Ismert útvonalakat, logikákat próbál, és kevésbé tesztel váratlan eseteket.
#### Mik a tesztelési alapelvek?
1. A tesztelés hibák jelenlétét mutathatja, de hibamentességet nem bizonyíthat.
2. A kimerítő tesztelés lehetetlen.
3. A tesztelést a lehető leghamarabb kell elkezdeni.
4. A hibák gyakran halmozódnak (nem egyenletesen oszlanak el).
5. A rovarirtás paradoxona: ha mindig ugyanazokat a teszteket futtatjuk, új hibákat nem találunk.
6. A tesztelés kontextusfüggő.
7. Téves hibaelhárítás: ha a hibákat kijavítjuk, új hibák kerülhetnek be.
#### Mit jelent az „alapvető tesztelési elv”, hogy „a kimerítő tesztelés lehetetlen”?
Nem lehet minden bemeneti kombinációt és futtatási utat kipróbálni → stratégiát kell alkalmazni (prioritás, kockázat).
#### Mit jelent az „alapvető tesztelési elv”, hogy „a hibák halmozódnak”?
A hibák általában nem egyenletesen oszlanak el a rendszerben, hanem bizonyos modulokban koncentrálódnak (pl. bonyolult, gyakran módosított részekben).
#### Mit jelent az „alapvető tesztelési elv”, hogy „a tesztelés a kontextustól függ”?
Más megközelítést igényel pl. egy biztonságkritikus repülőgép szoftver és egy mobiljáték tesztelése.


## 2. Tesztelés a szoftverfejlesztés életciklusán át
#### Mik a tesztszintek, és mi a különbség köztük?
1. Egységteszt (Unit Test) – kis kódrészek, függvények tesztje.
2. Integrációs teszt – modulok közötti kapcsolatok vizsgálata.
3. Rendszerteszt – a teljes rendszer vizsgálata a specifikáció alapján.
4. Felhasználói elfogadási teszt (UAT) – a végfelhasználó ellenőrzi, hogy a rendszer megfelel-e az üzleti igényeknek.
#### Miért nem érdemes mindig ugyanazokat a teszteseteket futtatni (regressziós torzítás)?
Mert ugyanazok a hibák fognak előjönni → új hibák rejtve maradnak. Időnként új teszteket kell hozzáadni.
#### Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
Egy adott modul, metódus vagy osztály funkcionális tesztje izoláltan.
Felelős: általában a fejlesztők írják és futtatják.
#### Mi a különbség a verifikáció és a validáció között?
Verifikáció = jól csináljuk? (A termék megfelel a specifikációnak?)
Validáció = jót csinálunk? (A termék megfelel a felhasználói igényeknek?)
#### Mik a tesztelési típusok, és mi a különbség köztük?
Funkcionális tesztelés – a rendszer mit csinál (követelmények alapján).
Nem-funkcionális tesztelés – a rendszer hogyan viselkedik (pl. teljesítmény, biztonság).
Változási tesztelés – regresszióteszt, új hibák megjelenése javítás után.
#### Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
Fehér doboz – belső kódstruktúrát ismerjük, logikai ágak, lefedettség alapján tesztelünk.
Fekete doboz – nem ismerjük a belső működést, csak a bemenetet és kimenetet vizsgáljuk.
Szürke doboz – részben ismerjük a belső struktúrát, de kívülről teszteljük.
#### Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
Rendszerteszt: ellenőrzi, hogy a rendszer a specifikáció szerint működik.
UAT: a felhasználók nézik meg, hogy a rendszer valóban kielégíti-e az üzleti igényeiket.
#### Mi a különbség a statikus és dinamikus tesztelés között?
Statikus tesztelés: futtatás nélkül történik (pl. kódfelülvizsgálat, dokumentum-ellenőrzés).
Dinamikus tesztelés: a szoftver futtatásával derítünk fel hibákat.


források:
https://astqb.org/istqb-foundation-level-seven-testing-principles/?
https://www.imbus.ca/software-testing/seven-principles-of-software-testing?
https://istqb.org/certifications/certified-tester-foundation-level-ctfl-v4-0/?
https://www.testing101.net/post/what-are-the-different-test-levels?
https://www.testing101.net/post/what-is-the-difference-between-verification-and-validation?
https://www.toolsqa.com/software-testing/istqb/software-testing-principles?