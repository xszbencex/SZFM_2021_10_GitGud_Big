# Koronavírus statisztikai előrejelző rendszer követelményspecifikáció

***1. Áttekintés***<br>
A projekt célja felmérni a koronavírus helyzetet, és a statisztikák alapján előrejelzéseket készíteni. A statisztikai adatokat a WHO felmérései szolgáltatják. Az előrejelzéseket egy megfelelő algoritmus kell, hogy biztosítja a meglévő adatokból. Ezen kívül szükséges az adatokat megjeleníteni gráfok, oszlopdiagrammok, kördiagrammok formájában. 
Szükséges adatok: 
- Megfigyelés dátuma
- Állam
- Ország/ Régió
- Utolsó frissítés
- Megbetegedt lakosok száma
- Halálesetek száma
- Gyógyultak száma


***2. Jelenlegi helyzet***<br>
- A **HealthLab Kft.** Magyarországon az egyik legnagyobb teszteléssel és adatfeldolgozással foglalkozó cég, amely szeretne felmérést készíteni a koronavírus járvány adataiból és előrejelzéseket készíteni. A járvány kiszámíthatatlansága rettegésben tartja az embereket, nehezíti az előre tervezést, hiszen a korlátozó intézkedések miatt lecsökken a mozgásterünk, alkalmazkodnunk kell a pandémiához. Az eddig feljegyzett adatok alapján, gépi tanuló algoritmusok segítségével elemezni tudjuk, hogy a fertőzésveszély, a járvány helyel-közel mikorra érheti el a tetőzést, milyen gyorsan terjedhet. Ezen információkat a feljegyzett megbetegedésekből, kigyógyulásokból illetve halálesetekből tudja kikövetkeztetni a rendszer. Ezen elemzések elvégzésével a cég hozzájárul a pandémiás időszak könnyebb átvészeléséhez.


***3. Vágyálom rendszer***<br>
- Ne csak egy, hanem minél több országra vonatkozóan történjen az adatfeldolgozás.
- Az előrejelzéseket egy adott országra le lehessen kérdezni.
- Fertőzések, megbetegedések, gyógyulások, halálozások gyakoriságát heti vagy havi lebontásban kezelni.
- Ezen felül oszlopdiagramos, kördiagramos, vonaldiagramos megjelenítés preferált.
- Különböző típusú esetek csoportosítása.
- Elvárás, hogy a megjelenő adatok egy laikus számára is jól átteknithetőek és érthetőek legyenek.

***4. A rendszerre vonatkozó szabályok***<br>
- Megbízható, hiteles adatbázisból származó adatokból kell az elemzést elkészíteni. (pl. WHO)
- Az eredmények reprodukálhatóak és könnyedén bővíthetőek legyenek.
- Legyen százalékos megjelenítés is.
- Ha weboldalon lesz a statistikai kimutatás, akkor a weboldal az összes elterjedt webböngészőn (Firefox, Chrome, Edge, Opera) igényesen nézzen ki és működjön megfelelően. A weboldal legyen modern, de egyszerű hogy a hozzá nem értők is értelmezni tudják a végkimenetelt.
- Elavult (deprecated) technológiákat kérjük ne használjanak, az időtállóság miatt
- A képek nagy felbontásúak legyenek, vízjel nélkül és png vagy jpg formátumúak
- A projektet ajánljuk valamilyen verziókezelő rendszer segítségével elkészíteni, a visszakövethetőség és az egyszerűbb csoportmunka miatt

***5. Jelenlegi üzleti folyamatok***<br>
- **5.1.** Koronavírus halálozási adatok hivatalos adatbázisból  =>  lekérés => elemzés 
- **5.2.** Lekért adatok feljegyzése =>  jelenleg az adatokból diagramok ábrázolása kézzel történik
- **5.3.** Több országból történő adatletöltés => Jelenleg lokálisan érkező adatok esetén nem lehet használható eredményt elérni, mivel dinamikusan történik a változás világviszonylatban
- **5.4.** Sok dimenziós adattábla használata csak a szükséges oszlopok felhasználásával (gyógyultak, betegek, halálozások, stb.) => jelenleg minden oszlop adatai kezelésre kerülnek, így az adatvizualizáció túl bonyolult, dimenziócsökkentés javasolt
- **5.5.** Statisztikai számítások (összegzés, eloszlás, maximum számítás, stb.) elvégzése beépített függvények segítségével => jelenleg papír alapú számítások
- **5.6.** Meglévő, feljegyzett adatokból egy tanuló modell felépítése, ami képes a jövőre vonatkozólag hiteles becslések számítására, azaz prediktálások elvégzésére => jelenleg csak a meglévő adatok állnak rendelkezésre, előrejelzés készítése bonyolult és körülményes 

***6. Igényelt üzleti folyamatok***<br>
- **6.1.** Egy olyan felület amely beolvassa az adatbázis adatait => adatfeldolgozás => elemzés => adatok kirajzolása programmal (diagramok)
- **6.2.** Elemzett adatok tovább vizsgálata => előrejelzés készítése egy adott országra vonatkozóan
- **6.3.** Adatok tisztitása
- **6.4.** Különböző típusú esetek csoportosítása
- **6.5.** Halálozási/megbetegedési/gyógyultsági ráta kiszámítása
- **6.6.** Előrejelzések készítése

<img src="images/Igényelt_üzleti_folyamatok.png" data-canonical-src=""/>

***7. Riportok***<br>
Kérdőív irányított riporthoz:

- Mit gondol, mit jelent Ön szerint az előrejelzés?
- Milyen előnyöket nyújtanak Önnek az előrejelzések?
- Milyen biztonsági szintet kell kielégítenie Ön szerint az adatok forrását tekintve?
- Milyen fő funkciókat vár el egy ilyen rendszertől?
- Milyen „vágyálom” funkciókat látna szívesen egy ilyen rendszertől?
- Kérem, írja körül, hogy jelenleg hogyan megy Önöknél egy adatfeldolgozás és elemzés? Milyen nehézségek adódtak ezeken?
- Kérem, soroljon előnyöket / hátrányokat a jelenlegi adatfeldolgozás  és a "vágyálom" adatfeldolgozás relációjában!
- Mit gondol, egy weboldal lehet alapja egy adafeldolgozó és megjelenítő, valamint előrejelző rendszernek?
- Milyen ablakok legyenek a rendszerben? Kérem, adjon képernyő terveket!
- Hallott már hasonló szolgáltatásról? Esetleg használja valamelyiket? Milyen tapasztalatai vannak?
- Ön szerint szükség van egy ilyen rendszere?
- Milyen költségei vannak a jelenlegi adatfeldolgozással kapcsolatban? Ön szerint csökkennének vagy nőnének ezek a költségek egy adatfeldolgozó és előrejelző rendszer esetén?

***8. Követelménylista***<br>
A statisztikai programban megjelenő funkciók táblázatba foglalása és al-funkciók leírása.

|   Modul   | ID |         Név         | Kifejtés |
|-----------|----|---------------------|----------|
|Elemző rendszer         | K1 | Adatok | Csak ellenőrzött, hivatalos adatokbázisokból nyert adatokkal dolgozhat a rendszer. |
|Elemző rendszer         | K2 | Adatfeldolgozás | Az adatbázisból szükséges adatok: Világ országai, adott ország lakosainak létszáma,  országonkénti megbetegedések száma heti rendszerességgel, országonkénti gyógyultak száma heti rendszerességgel, országonkénti tesztelések száma heti rendszerességgel, országonkénti pozitív tesztesetek száma, megbetegedő lakosok átlag életkora. |
|Elemző rendszer         | K3 | Előrejelzés | Az adatokból előrejelzést egy adott országra vonatkozóan kell készíteni hogy ne igényeljen hosszú időt az adatfeldolgozás |
|Elemző rendszer         | K4 |  ... |...|
|Jogi szabályok| K5 |Jogi nyilatkozatok   |Adatvédelmi nyilatkozat, GDPR, ASZF, szükség esetén Cookie szabályzat feltüntetése a weblapon. (?) |
|Felület       | K6 | ... |...|
|Felület       | K7 |...  |...|
|Felület       | K8 |...   |...|
|Felület       | K9 |...|...|
|Felület       | K10 |... |...|

***9. Fogalomszótár***<br>
**Mesterséges intelligencia** - lehetővé teszi a technika számára, hogy érzékelje környezetét, foglalkozzon azzal, amit észlel, problémákat oldjon meg, és konkrét cél elérése érdekében tervezze meg lépéseit. A számítógép nemcsak adatokat fogad (már előkészített vagy összegyűjtött adatokat érzékelőin, például kameráján keresztül), hanem fel is dolgozza azokat és reagál rájuk.

**Gépi tanulás** - a mesterséges intelligencia olyan ága, olyan rendszerekkel foglalkoznak, melyek tanulni képesek, azaz tapasztalatokból tudást generálnak. A gyakorlatban ez azt jelenti, hogy a rendszer példa adatok, minták alapján képes önállóan, vagy emberi segítséggel szabályszerűségeket/szabályokat felismerni/meghatározni.

**Mély tanulás** - a gépi tanulási technikák egy alcsoportja, amiben mesterséges neurális hálózatokat (Neural Networks) használunk.

**Adat** - tények, fogalmak olyan megjelenési formája, amely alkalmas emberi eszközökkel történő értelmezésre, feldolgozásra, továbbításra. 

**Adathalmaz** - információk összessége, sokasága. 

**Adatelemzés** - meglévő adatok feldolgozása, értelmezése, összekapcsolása.

**Predikcíó** - a már megismert és bizonyított törvényszerűségekből levonható következtetéseken alapuló előrejelzés, jóslat.

**Inicializáció** - kezdőértékek meghatározása.