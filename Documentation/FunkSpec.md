***1. Áttekintés***<br>
A projekt célja felmérni a koronavírus helyzetet, és a statisztikák alapján előrejelzéseket készíteni. A statisztikai adatokat a WHO felmérései szolgáltatják. Az előrejelzéseket egy megfelelő algoritmus kell, hogy biztosítja a meglévő adatokból. Ezen kívül szükséges az adatokat megjeleníteni gráfok, oszlopdiagrammok, kördiagrammok formájában. Szükséges adatok: Világ országai, adott ország lakosainak létszáma,  országonkénti megbetegedések száma heti rendszerességgel, országonkénti gyógyultak száma heti rendszerességgel, országonkénti tesztelések száma heti rendszerességgel, országonkénti pozitív tesztesetek száma, megbetegedő lakosok átlag életkora.

***2. Jelenlegi helyzet***<br>
 A **HealthLab Kft.** Magyarországon az egyik legnagyobb teszteléssel és adatfeldolgozással foglalkozó cég, amely szeretne felmérést készíteni a koronavírus járvány adataiból és előrejelzéseket készíteni.

***3. Követelménylista***<br>
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


***4. Jelenlegi üzleti folyamatok modellje***<br>

 


  
***5. Igényelt üzleti folyamatok modellje***<br>

  

***6. Használati esetek***<br>
-FELHASZNÁLÓ: Az adatfeldolgozó rendszerbe belépve, jogosultsága van a mezők kitöltésére és adatmegjelenítési beállítások kiválasztására, valamint statisztikai előrejelzések futtatására.<br>
-ADMIN: Az ADMIN beléphet mindegyik más szerepkörbe,
hogy a hibamentes működést ellenőrizhesse. Az Admin
feladata a rendszer problémamentes működtetése. Ez egyben jár azzal,
hogy az egész rendszerhez van hozzáférése.

***7. Képernyő tervezete***<br>

Az űrlap egyszerűsített tervezete okostelefon képernyőn:<br>
<img src="" data-canonical-src="" width="445" height="681" />

 
 ***8. Forgatókönyv***<br><br>
 **Szereplők:**<br><br>
Futási időben két szereplő figyelhető meg. Az
első szereplő maga a futó ALKALMAZÁS. (weben/androidon)
Ezzel van interakcióban a második szereplő, maga a FELHASZNÁLÓ, aki ...
