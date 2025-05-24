🎯 1. Mi az a szoftvertechnológia?
Professzionális szoftverfejlesztés módszertana.

Célja: funkcionalitás, minőség, költség és határidő garantálása.

A szoftver nemcsak kód, hanem: programok, dokumentációk, konfigurációk és adatok együttese.

✅ 2. Minőségi mutatók (quality characteristics)
Karbantarthatóság (maintainability) – könnyen módosítható, bővíthető

Megbízhatóság, biztonság (dependability, security) – hibák, támadások elleni védelem

Hatékonyság (efficiency) – erőforrás-használat, válaszidő

Használhatóság (usability) – egyszerűség, tanulhatóság

👷 3. Szoftvertechnológiai projekt szerepei
Projektmenedzser – vezetés, erőforrás, minőség, dokumentáció

Termékgazda – üzleti értékek, prioritás

Programgazda – ütemezés, nyomon követés

Tervező – technikai architektúra

Fejlesztő

Tesztelő / QA – tesztelés, ellenőrzés

🔁 4. Szoftver életciklus – fő fázisai
Specifikáció – mit kell csinálni

Tervezés és implementáció – hogyan működjön

Verifikáció és validáció – tesztelés, megfelelés

Evolúció – hibajavítás, bővítés

📄 5. Specifikáció részlépései
Megvalósíthatóság elemzése

Követelmények feltárása és dokumentálása

Követelmény specifikáció

Követelmény validáció → eredmény: SRS (Software Requirements Specification)

🧠 6. Tervezés & implementáció
Szoftver rendszerterv készítése (statikus + dinamikus)

Használható prototípus (horizontális: UI, vertikális: funkcionalitás)

Verziókezelés, IDE, tesztelés

🧭 7. Programozási paradigmák
Procedurális, objektumorientált, funkcionális, logikai, adatfolyam-alapú

Meghatározzák a kód stílusát, nyelvválasztást, absztrakciókat

✔️ 8. Validáció & evolúció
Validáció: megfelel a követelményeknek?

Evolúció: új igényekhez illesztés (élettartam 80%-a!)

📦 9. Dokumentáció típusai
Felhasználói: üzembe helyezés, funkciók

Fejlesztői: technikai részletek, implementáció

⏱ 10. Ütemterv & mérföldkövek
Hierarchikus feladatszerkezet

Függőségek, felelősök, határidők

Mérföldkő = ellenőrizhető cél, státusz pont

💡 11. UML 5 nézete
Használati nézet – user funkciók (use case)

Szerkezeti – osztályok, komponensek

Dinamikus – viselkedés, állapot, szekvencia

Implementációs – kód, komponensek

Környezeti – hardver, szoftver kapcsolatok

🛠️ 12. Hasznos eszközök
Project tracking

CASE tool

IDE

Version Control (Git)

CI/CD tools

🔁 13. Fejlesztési modellek
🔹 Vízesés (Waterfall)
Lineáris, előre definiált

✅ Strukturált

❌ Nem kezeli változásokat

🔹 Spirális (Spiral)
Prototípus + kockázatvezérelt

✅ Jó kockázatkezelés

❌ Költséges

🔹 Inkrementális
Funkciók lépésről lépésre

✅ Gyors feedback

❌ Átláthatóság gyenge

⚡ 14. Agilis fejlesztés
Inkrementális, gyors kiadás (continuous delivery)

Értékek (Agilis Kiáltvány szerint):

Egyének > folyamatok

Működő kód > dokumentáció

Ügyfél együttműködés > szerződés

Reagálás > terv követése

🌀 15. Scrum módszer
Sprint (2–4 hét) + tervezés + review + retrospective

Nincs projektmenedzser → van Scrum Master

Product backlog + sprint planning + daily stand-up

📚 16. Modellek csoportosítása
Típus Cél
Terv-vezérelt Minőség, stabilitás
Agilis Rugalmasság, egyszerűség
Formális Bizonyítható helyesség

<!-- 2 -->

🎯 1. Mi az a specifikáció és miért fontos?
Célja: A szoftver céljainak, funkcióinak, korlátainak és elvárásainak pontos meghatározása felhasználói és fejlesztői oldalról is.

Eredménye: A Software Requirements Specification (SRS) dokumentum.

🔄 2. A specifikáció lépései:

1. Megvalósíthatósági elemzés (Feasibility Study)
   Vizsgálja, hogy:

Lehetséges-e a megvalósítás technikailag és gazdaságilag?

Milyen erőforrások szükségesek (humán, szoftver, hardver)?

Milyen lesz az üzemeltetés, karbantartás költsége?

Gyors és olcsó elemzés → ha egyedi projekt: ajánlattétel követi.

2. Követelményfeltárás és -elemzés (Elicitation & Analysis)
   Három lépés:

Kutatás: interjúk, meglévő rendszerek vizsgálata.

Osztályozás: csoportosítás, alrendszerekhez rendelés.

Prioritás: fontosság szerinti sorrend, feleslegesek kiszűrése.

Nehézségek:

Vevő bizonytalan / nem informatika szakértő

Eltérő igények, változó környezet

3. Követelmények típusai:
   📌 Funkcionális követelmények:
   Mit csinál a rendszer: funkciók, reakciók, viselkedés

📌 Nem funkcionális követelmények:
Hogyan viselkedjen a rendszer. Pl.:

Hatékonyság (Efficiency) – erőforrás-használat

Megbízhatóság (Dependability) – hibakezelés, robusztusság

Biztonság (Security) – hozzáférésvédelem

Hordozhatóság (Portability) – platformfüggetlenség

Használhatóság (Usability) – könnyen kezelhető

📌 Menedzselési követelmények:
Környezet (kell-e más szoftver, milyen gépen fut)

Fejlesztési környezet, nyelvek, módszertan

Működési paraméterek (idő, gyakoriság)

📌 Külső követelmények:
Törvényi, etikai, jogi megfelelés

🧩 3. Példák – esettanulmányok
🥪 Marika néni kávézója
Funkciók:

Étel/ital hozzáadás

Rendelések, törzsvásárlói szám

Statisztikák (nap/hónap/törzsvásárló)

Adatmentés szöveges fájlba

Nem-funkcionális példa:

Csak Windows 7+, nem garantált adatbiztonság

Felhasználóbarát, de kevés adatot kezel

🃏 Memory játék
Aktor: játékos

Funkciók:

Kártyacsomag és név választás, játék indítás

Két kártya felfordítása (ha egyezik → marad, ha nem → vissza)

Diagramok: include, precedes relációk

🏠 Utazási ügynökség
Aktor: felhasználó, admin

Webes felület: keresés, foglalás

Admin: új apartman hozzáadás, képek feltöltése

Adatbázis műveletek: ütközéskezelés, tárolás, lekérdezés

🗂 4. Használati esetek (Use Cases)
Aktor: aki használja a rendszert (pl. Büfés, Játékos, Admin)

Funkció: a rendszer szolgáltatásai

Kapcsolatok:

include: része egy másiknak (kötelező)

extend: opcionális bővítés

precedes: sorrend (előfeltétel)

invokes: következmény

✍️ 5. Felhasználói történetek (User Stories)
Formátum:

css
Másolás
Szerkesztés
As a [user role], I want to [goal], so that [reason]
Bővítés Given–When–Then formában:

Given – adott környezet

When – esemény

Then – elvárt válasz

Példa:
As a Büfés, I want to add an item to the order.

Given the item menu is opened

When I enter a valid name and price

Then it gets added to the order

✅ 6. Követelmény validáció
Cél: A specifikáció konzisztens, valószerű, ellenőrizhető legyen

Eredmény:

Prototípus (gyors teszteléshez)

Tesztesetek (végső validációhoz)

📄 7. Követelmény-leírás (SRS dokumentum felépítése)
Előszó

Bevezetés

Fogalomtár

Követelmények – felhasználói

Rendszer architektúra

Követelmények – fejlesztői részletes leírás

Rendszermodellek (pl. UI mockup, adatmodell)

Evolúció (jövőbeli bővítések)

Függelék

Tárgymutató

<!-- 3 -->

🎯 1. Objektumorientált tervezés alapjai
🔹 Objektumok, osztályok
Objektum = valóság absztrakciója: adat + működés

Osztály = objektumok sablonja (azonos funkció + állapot)

Elemzés során:

Azonosítjuk a funkciókat → ezekhez rendeljük az adatokat → ebből lesznek az osztályok

🧱 2. Tervezési fázisok
Többlépcsős, iteratív folyamat

Minden fázisban lehet:

új osztály bevezetése

meglévő pontosítása vagy felosztása / összevonása

🧭 3. SOLID alapelvek
Rövidítés Elv neve Jelentés
SRP Single Responsibility Egy osztály csak egy felelősséggel bírjon
OCP Open/Closed Nyitott bővítésre, zárt módosításra
LSP Liskov Substitution Altípus helyettesíthetőség
ISP Interface Segregation Sok kicsi interfész, ne egy nagy
DIP Dependency Inversion Az absztrakciótól függjünk, ne a konkréttól

🧱 4. Szoftverarchitektúra
Elsődleges döntések összessége, amelyek a rendszer szerkezetét, viselkedését, skálázhatóságát, stb. meghatározzák

Architekturális minta: egész rendszer struktúrája (pl. MVC)

Tervminta (design pattern): kisebb részek kapcsolata (pl. Factory, Observer)

🧱 5. Architektúratípusok
Monolitikus
Minden egy blokkban: adatkezelés + GUI + logika együtt

Modell / Nézet (Model/View)
Modell: alkalmazáslogika (állapot + adatok)

Nézet: GUI + eseménykezelés

Modell nem ismeri a nézetet, de a nézet figyelhet modellre (pl. observer)

🧪 6. Esettanulmány: Marika néni kávézója
Objektumok:

Item (szülőosztály) → Hamburger, Ufo, Pancake, Tea, Coke, Orange

Order → tételek listája, dátum, kártyaszám

Menu → rendelések listája, menü logika

Adattárolás:

Fájlformátum: .dat, CSV-szerű (pontosvessző + sortörés)

<rendelés_id>;<dátum>;<kártyaszám>;<tételek_száma>

🃏 7. Esettanulmány: Memory játék
Modell osztályok:

GameManager, CardPack, Player

Nézet osztályok:

MainWindow, GameWidget, ConfigurationDialog, ImageButton

Adattárolás:

name.txt – csomag neve

back.png – hátlap

0.png, 1.png, … – előlapok képei

🏨 8. Esettanulmány: Utazási ügynökség
Felhasználói kliens:

Webes kliens (JRE + weblap)

Asztali alkalmazás (JRE)

Szerver oldalon:

Webszolgáltatás (Spring) → DB közvetítés

Adatbázis séma:

city, building, apartment, customer, stb.

📦 9. UML diagramok
Diagram Cél
Csomagdiagram (package) Logikai egységek, csomagok kapcsolatai
Komponensdiagram Komponensek, interfészek, kapcsolat (pl. SQL, API)
Telepítési diagram (deployment) Hardver/szoftver elemek elhelyezése, csomópontok
Osztálydiagram Statikus szerkezet
Szekvencia/állapot diagram Dinamikus működés (pl. események, állapotok)

🧾 10. Rendszerterv (Software Design Description – SDD)
Felépítése:
Előszó

Bevezetés

Fogalomtár

Architektúra (UML + minta)

Adattervezés

Rendszerterv (osztályok, állapotok, interfészek)

Felület

Implementációs ajánlások

Függelék

Tárgymutató
