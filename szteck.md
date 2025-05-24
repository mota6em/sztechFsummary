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

<!-- 4 -->

📕 ea04 – Objektumorientált tervezési szempontok és minták

1. SOLID alapelvek
   SRP (Single Responsibility Principle): Egy osztály csak egyetlen felelősséggel bírjon.
   Példa: könyvkeresést (locate) a könyvtáros használja, kiíratást (print) az olvasó. Ezek külön osztályokban: BookLocator, BookPrinter.

OCP (Open/Closed Principle): A kód legyen nyitott bővítésre, de zárt módosításra.
Példa: minden Shape (pl. Circle, Rectangle) maga számolja ki a getArea(), így nem kell új if-et írni új alakzat esetén.

LSP (Liskov Substitution Principle): Egy osztály altípusa helyettesíthető az eredetivel anélkül, hogy hibás működést okozna.
Példa: Square nem felel meg a Rectangle öröklésnek, mert setHeight() → setWidth().

ISP (Interface Segregation Principle): Egy osztály csak azokat a műveleteket lássa, amiket használ.
Példa: EmailClient csak az Emailable-t használja, PhoneClient csak a Callable-t.

DIP (Dependency Inversion Principle): A felsőbb osztályok absztrakt interfészekre épüljenek, ne konkrét implementációkra.
Példa: Client a Calculator interfészt kapja konstruktorban, nem példányosít LogCalculator-t.

2. Függőség befecskendezés (Dependency Injection)
   A kliens nem példányosítja a szolgáltatást, hanem külső komponens adja át neki.

Lehetséges formák: konstruktor, metódus, vagy interfész alapú injektálás.

Példa: Injector adja a Client-nek a Calculator-t.

3. Tervezési minták
   Factory – példányosítási logika elrejtése

Factory Method – leszármazott határozza meg, mit gyárt

Abstract Factory – kapcsolódó objektumok gyártása egy helyen

Command – egy tevékenység (pl. Execute) objektummá alakítása, amit az Invoker hív

4. Architektúrák
   Monolitikus – minden egy fájlban; rosszul skálázható

Model–View – modell a logika és adat, nézet az UI; nem elég elkülönített

3-Tier –

Nézet (View)

Üzleti logika (Logic)

Perzisztencia (Data)

MVC –

Model: logika és állapot

View: felület, deklaratív

Controller: feldolgozza az eseményeket
Webes rendszerekben különösen elterjedt.

5. Adatkötés és állapotok
   Három fő adatállapot:

Display state – felhasználó által látott

Session state – programban tárolt

Record state – adatbázisban mentett

Adatkötés (Data Binding):

Automatizált szinkronizálás Binding objektummal

GetState(), SetState(), Convert()

Nézet ismerheti a bindinget, modell nem

Figyelő minta segít a szinkronban

6. Figyelő minta (Observer)
   Subject: értesít minden figyelőt (Notify)

Observer: reagál a változásra (Update)

Modell nem ismeri a vezérlőt vagy nézetet – csak eseményt küld

<!-- 5
 -->

📘 ea05 – Projektmenedzsment eszközök és verziókezelés

1. Fejlesztést támogató eszközök
   Projekt tracking system – dokumentálás, feladatkövetés

CASE tool – fejlesztési folyamat, felelősségek nyomon követése

IDE – integrált fejlesztési környezet

Revision Control System (VCS) – kódváltozások követése

CI rendszer – hibák automatikus észlelése fejlesztés során

2. Projektmenedzsment eszköz funkciói
   Ütemterv, kockázatkezelés

Dokumentáció létrehozása és frissítése

Feladatkezelés (ticket/issue – bug, feature, task, documentation)

Kommentelés, határidők, felelősök hozzárendelése

Verziókezelés és code review

3. Népszerű eszközök
   Trac – Python, MySQL/PostgreSQL/SQLite

Redmine – Ruby on Rails

Azure DevOps – Microsoft (TFVC, Git)

YouTrack – JetBrains, Java + NoSQL (Xodus)

GitHub, GitLab, Bitbucket – cloud-alapú hosting

4. GitLab
   Webes felület, projektmenedzsment + CI/CD integráció

Két változat:

Community Edition – self-hosted, nyílt forráskód

Enterprise Edition – vállalati funkciók

ELTE GitLab: https://szofttech.inf.elte.hu/

feladatkövetés, wiki, forráskódkezelés, automatikus tesztelés

5. Verziókövetés célja
   Többfejlesztős munka szinkronizálása

Állapotmentés (commit), visszavonás, visszaállítás

Ágkezelés: branch, merge, tag

Fájl- és sor-szintű változáskövetés

Konfliktuskezelés + diff

6. Verziókezelő generációk
1. generáció – Lokális (SCCS, RCS), fájlonkénti, zár alapú

1. generáció – Központi (CVS, SVN), kliens-szerver modell

1. generáció – Elosztott (Git, Mercurial), minden kliensnél teljes repo

1. Git parancs alapok
   git init, clone, add, commit, push, pull

git branch, checkout, merge

.gitignore fájl a kizárásokhoz

Konfliktus: <<<<<<<, =======, >>>>>>>

8. Nagy fájlok kezelése
   Ne verziókezelj: build fájlok, binárisok, IDE beállítások

.gitignore – minták GitHub-ról: github/gitignore

Git LFS – Nagy fájlokat külső táron tárol (linkelve)

9. Branch modellek
   GitFlow: master, develop, feature, release, hotfix

GitHub Flow: master + feature, gyors release

GitLab Flow: master, staging, production különválasztva

10. Támogatott eszközök
    GUI-k: TortoiseGit, SourceTree, GitKraken, SmartGit

IDE-k: IntelliJ IDEA (VCS menü), NetBeans (Team menü)

<!-- 6-->

📗 ea06 – Build Systems (Ant, Maven, Gradle)

1. Why build systems?
   Manual compiling (e.g. javac, jar) is error-prone, slow, and hard to scale.

Build systems solve:

Compilation automation

Dependency management

Packaging (JAR, WAR, etc.)

Testing and reporting

Deployment automation

2. Ant (Imperative, XML-based)
   File: build.xml

Key concepts:

<project>: defines name, default target, basedir

<target>: defines a build step (e.g. compile, jar, clean, run)

<property>: key-value pairs, reusable via ${key}

Typical tasks:

prepare: create folders (e.g. mkdir dir="classes")

compile: compile Java with <javac>

jar: package classes into .jar with manifest

clean: delete output files/folders

test: run JUnit tests with <junit> and <batchtest>

run: launch JAR or class with <java>

Used in NetBeans (default) – auto-generates build-impl.xml for hooks

3. Maven (Declarative, XML-based)
   File: pom.xml

Core concept: POM = Project Object Model

groupId, artifactId, version (GAV)

Build config, test config, dependencies

Lifecycle phases:

validate, compile, test, package, verify, install, deploy

mvn install: compiles, tests, packages, installs locally

mvn clean install: deletes old builds then runs full build

Dependencies:

Declared in <dependencies> block

Resolved from Maven Central → stored in local repo (~/.m2/repository)

Scoped: compile, test, runtime, etc.

Plugins:

Extend functionality, e.g. maven-javadoc-plugin, surefire for test reports

Supports modular projects:

Parent POM + <modules>

4. Gradle (Script-based, Groovy/Kotlin DSL)
   File: build.gradle (or build.gradle.kts)

Features:

Combines Ant’s flexibility + Maven’s conventions

Faster builds (incremental)

Uses tasks (task name { doLast { ... } })

dependsOn defines task order

Plugins:

java – build, test, jar, clean

application – for executables (mainClass = ...)

Dependency config:

groovy
Másolás
Szerkesztés
repositories { mavenCentral() }
dependencies {
implementation "..."
testImplementation "junit:junit:4.13.2"
}
Gradle Wrapper (gradlew) ensures version consistency across machines

Supported in IntelliJ IDEA, NetBeans

5. Summary of Tools
   Tool Language Style File Key Feature
   Ant Java Imperative build.xml Fine-grained task control
   Maven Java Declarative pom.xml Convention over config
   Gradle Any DSL-based build.gradle Fast, flexible, modern
