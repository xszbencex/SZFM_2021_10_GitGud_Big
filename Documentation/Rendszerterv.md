# Rendszerterv

***1. A rendszer célja***<br>
A rendszer célja felmérni a koronavírus helyzetet, és a statisztikák alapján előrejelzéseket készíteni. A statisztikai adatokat a WHO felmérései szolgáltatják. Az előrejelzéseket egy megfelelő algoritmus kell, hogy biztosítja a meglévő adatokból. Gépi tanuló algoritmusok segítségével elemezni tudjuk, hogy a fertőzésveszély, a járvány helyel-közel mikorra érheti el a tetőzést, milyen gyorsan terjedhet. Ezen információkat a feljegyzett megbetegedésekből, kigyógyulásokból illetve halálesetekből tudja kikövetkeztetni a rendszer. Ezen kívül szükséges az adatokat megjeleníteni gráfok, oszlopdiagrammok, kördiagrammok formájában.  
Szükséges adatok: 
- Megfigyelés dátuma
- Állam
- Ország/ Régió
- Utolsó frissítés
- Megbetegedt lakosok száma
- Halálesetek száma
- Gyógyultak száma

***2. Projektterv***<br>
**Projekt munkatársak és felelőségek:**

Backend munkálatok: 
- Pete Balázs
- Szabó Bence
- Szimeonov Viktória
- Tóth Csenge Beatrix
- Tóth Zoltán

Feladatuk a funkciók létrehozása és megvalósítása.

| Funkció / Story | Feladat / Task | Prioritás | Becslés | Aktuális becslés | Eltelt idő | Hátralévő idő |
|-----------------|----------------|-----------|---------|------------------|------------|---------------|
| Követelmény specifikáció | | 0 | 12 | 12 | 12 | 0 |
| Funkcionális specifikáció | | 0 | 12 | 12 | 12 | 0 |
| Rendszerterv | | 0 | 16 | 16 | 16 | 0 |
| Fejlesztés | Google Colab | 1 | 12 | 12 | 12 | 0 |
| Tesztelés | | 1 | 16 | 16 | 10 | 6 |
| Értékelés | | ? | ? | ? | ? | ? |

***3. Üzleti folyamatok modellje***<br>

***4. Követelmények***<br>
Követelmények, funkciók, melyek a megfelelő működéshez elengedhetetlenek.
- Funkcionális követelmények:
  - Csak ellenőrzött, hivatalos adatokbázisokból nyert adatokkal dolgozhat a rendszer.
  - Az adatokból előrejelzést egy adott országra vonatkozóan kell készíteni hogy ne igényeljen hosszú időt az adatfeldolgozás
  - Választási lehetőség, hogy melyik országra szeretnénk előrejelzést készíteni.
- Nem funkcionális követelmények:
  - A rendszer minimális válaszidőn belül feldolgozza az adatokat.
  - Biztonságos működés.
  - Könnyű karbantarthatóság.
  - Működőképesség, használhatóság.
  - Adatok megbízhatósága és rendelkezésre állása.
- Törvényi előírások, szabványok:
  - GDPR-nak, ÁSZF-nek való megfelelés.

***5. Funkcionális terv***<br>
**<ins>Rendszer szereplők:<ins>**
- Admin
- Felhasználó

**<ins>Rendszerhasználati esetek és lefutásaik:<ins>**<br>
ADMIN:
- Beléphet bármilyen szereplőként teljes hozzáférése van a rendszerhez
- Tesztek létrehozása, törlése, módosítása

FELHASZNÁLÓ:
- Képes beállítani, hogy melyik országra legyen előrejelzés a koronavírus megbetegedések számára.
- Képes kirajzoltatni a preferált beállításoknak megfelelő diagrammokat.
- Képes megjeleníteni a preferált adathalmazt.


***6. Fizikai környezet***<br>
  
- A rendszer Android és web platformon, hordozható eszközökön (okostelefonok, táblagépek) futtatható.
- Az összes elterjedt webböngészőn (Firefox, Chrome, Edge, Opera) megfelelően működik.
- Nincsenek megvásárolt komponenseink.
- Fejlesztői eszközök:
  - Google Colab

***7. Architektúrális terv***<br>
  ![uml_diagram](images/uml_diagram.png)

***8. Adatbázis terv***<br>
<img src="images/dataset.png" data-canonical-src="" />

***9. Implementációs terv***<br>

***10. Karbantartási terv***<br>

***11. Tesztterv***<br>

***12. Telepítési terv***<br>
**Webes alkalmazás:**
    A szoftver webes felületéhez csak egy ajánlott böngésző telepítése szükséges (Google Chrome, Firefox, Opera, Safari) illetve egy Google fiókos regisztráció, külön szoftver nem kell hozzá. A weboldalra közvetlenül az internetről kapcsolódnak rá a kliensek.
    
**Mobil alkalmazás:**
    A szoftver hordozható eszközökön (okostelefonok, táblagépek) történő futtatásához a Google Colab Androidos webnézegető alkalmazásának letöltése javasolt, illetve egy érvényes Google fiók. Az alkalmazás lehetővé teszi a Google Colab használatát, reklám- és hirdetésmentesen.
