📘 Telekommunikációs Hálózatok – Lecture 1 Summary (For Exam)
🌐 1. What is the Internet?
Network of networks (globally connected, no central control)

Components:

End devices (hosts)

Switches & routers

Transmission media (cables, wireless, optical fiber)

📦 2. Packet-Switched vs Circuit-Switched
Feature Packet-Switched (Internet) Circuit-Switched (Phone)
Resource use On demand Reserved in advance
Efficiency High for bursty traffic Low for bursty traffic
Setup time No setup Needs connection setup
Example Data transfer Voice call

Protocol for circuit-switching: RSVP (Resource Reservation Protocol)

📶 3. Network Access Technologies
DSL (phone line): asymmetric bandwidth (higher download)

CATV (cable TV): shared medium, also asymmetric

Ethernet: LAN technology (1, 10, 100 Gbps, symmetric)

Other types: FTTH, Mobile, Satellite, Infiniband

📊 4. Resource Sharing Methods
Two main models:
Előre foglalás (Reservation) → fixed resources, wasteful if not used

Igény szerinti (On-demand) → dynamic, better utilization

Key ratios:
P/A (Peak/Average rate):

Low → reservation is OK (e.g., voice)

High → reservation is wasteful (e.g., data, bursty)

🧠 5. Important Concepts
Hoszt: network-connected device

Flow: logically grouped communication (e.g., TCP stream)

Multiplexálás:

Flow-level (reservation)

Packet-level (on demand)

Topologies: mesh, ring, star → Internet uses a hybrid with switch-based networks

🕸 6. Internet Structure
ISP hierarchy:

Tier 1: no upstream provider

Tier 2: connects T1s and T3s

Tier 3: local access (home/uni/company)

Peering: direct inter-ISP connection

IXP: internet exchange point to reduce costs

🛑 7. Risks and Outages
BGP misconfiguration → massive traffic rerouting (e.g., 2017 incidents)

Internet shutdowns → political reasons in some countries

Human errors → 50–80% of network outages

🧾 8. Exam Format
Must pass practice part to take the exam

📘 3 parts:

English terms test (20 Q, pass = 50%, no points)

MCQ Test (60 Q, 60 mins, min 30 pts)

30–44 pts = 2

45–59 pts = 3

Oral exam required for 4–5

<!-- 2 -->

📘 Előadás 2 – Kommunikáció, Protokollrétegek, Teljesítmény (Vizsgára)
🔄 1. Kommunikáció az Interneten
Cél: Távoli folyamatok (pl. Alice & Bob) adatot tudjanak cserélni

Protokoll: szabályrendszer (ki beszél, mikor, hogyan válaszol)

Példa: WoW kliens–szerver → API-kon keresztül történik

🧱 2. Modularitás & Rétegzés
Modularitás segíti:

hibaelhárítást

frissítést

skálázhatóságot

Protokollok rétegekre bontva, minden réteg egy másikat használ, és egy másiknak szolgáltat

🧩 3. Modell típusok
🔹 TCP/IP modell (4 réteg)
Link, Internet, Szállítási, Alkalmazási

🔹 Hibrid modell (5 réteg)
Fizikai, Adatkapcsolati, Hálózati, Szállítási, Alkalmazási

🔹 OSI modell (7 réteg)
Fizikai → Adatkapcsolati → Hálózati → Szállítási → Ülés → Megjelenítési → Alkalmazási

📦 4. Rétegek funkciói
Réteg Szolgáltatás Példák
Alkalmazási Felhasználói alkalmazások HTTP, FTP, DNS
Megjelenítési Adatformátum-átalakítás ASCII↔Unicode
Ülés Kapcsolat menedzsment (ritka, nincs konkrét protokoll)
Szállítási Megbízható továbbítás, multiplexálás TCP, UDP
Hálózati Útvonalválasztás, IP címzés IPv4, IPv6
Adatkapcsolati Keretezés, MAC, megbízhatóság Ethernet, WiFi
Fizikai Bitek átvitele Optikai kábel, koax, réz

📌 PDU-k:

Alkalmazás: üzenet

Szállítás: szegmens

Hálózati: csomag

Adatkapcsolat: keret

Fizikai: bitek

📦 5. Beágyazás (Encapsulation)
Minden réteg hozzáad egy fejlécet az előzőhöz

Példa: HTTP → TCP → IP → Ethernet → Fizikai átviteli egység

💻 6. Hol vannak a rétegek?
Hosztok (PC, szerver): minden réteg

Router: L3 + L2 (IP + Ethernet)

Switch: csak L2 (Ethernet)

⏱ 7. Hálózati jellemzők
Teljes késleltetés:
Másolás
Szerkesztés
= átviteli + terjedési + feldolgozási + várakozási késleltetés
Átviteli késleltetés:
Másolás
Szerkesztés
= csomag mérete / sávszélesség
Terjedési késleltetés:
Másolás
Szerkesztés
= távolság / jelterjedési sebesség
Várakozási késleltetés (queueing):
függ a forgalomtól

intenzitás = (La / R) (La: érkezési sebesség, R: sávszélesség)

Feldolgozási késleltetés:
fejléc elemzése → általában kicsi

❌ 8. Csomagvesztés & Átviteli sebesség (Throughput)
Veszteség: ha a buffer megtelik

Átviteli sebesség:

bash
Másolás
Szerkesztés
= adat mennyisége / idő
A bottleneck link határozza meg a maximumot

⚠️ Aranyszabály
Tervezd úgy a várakozási rendszert, hogy az intenzitás << 1 legyen
(különben végtelen sor → nagy késés, elvesztés)

🤔 Tipikus vizsgakérdések
Sorold fel a TCP/IP vagy OSI rétegeket

Magyarázd el az encapsulation-t

Milyen késleltetési típusok vannak?

Melyik réteg mit csinál?

<!-- 3 -->

Előadás 3 – Fizikai réteg (Vizsgára)
🧠 1. Fogalma és szerepe
Szolgáltatás: bit szintű adatátvitel fizikailag összekötött eszközök között

Interfész: egyes bitek átvitele

Protokoll: kódolási séma, feszültségszintek, időzítés

Példák: koaxiális kábel, optikai kábel, rádióadó

⚙️ 2. Alapfogalmak
Digitális világ (0,1) ≠ analóg világ (folytonos jelek)

Bit: alacsony/magas feszültség

ASCII kódolás: pl. ‘b’ → 01100010

Adatátvitel során zaj, elnyelődés, torzítás léphet fel

🔢 3. Szimbólumok és Adatráta
Több bitet 1 szimbólummal lehet ábrázolni (pl. 4 szimbólum → 2 bit/szimbólum)

BAUD: szimbólumok száma / másodperc

Adatráta = BAUD × log₂(n szimbólum)

📡 4. Átviteli közegek
➤ Vezetékes:
Sodort érpár: UTP/STP (telefonhálózat)

Koax kábel: jobb sávszél, analóg/digitális

Optikai kábel: fényimpulzusok, magas sebesség

➤ Vezeték nélküli:
Rádiófrekvencia: olcsó, nagy hatótáv

Mikrohullám: egyenes vonalon, olcsó

Infravörös/lézer: rövidtáv, időjárásfüggő

🛰 5. Műholdas kommunikáció
Geoszinkron: 35,800 km, ~270 ms késés

Közepes pálya: ~10 műhold, 35–85 ms

Alacsony pálya: ~50 műhold, 1–7 ms késés

🔁 6. Kódolási technikák
Kódolás Jellemző
NRZ 1 → magas, 0 → alacsony, de szinkron probléma lehet
Manchester Minden bithez átmenet (megoldja szinkront)
NRZI 1 → váltás, 0 → nem vált, de 0-kal gond lehet
4b/5b 4 bit → 5 bitre kódolás, NRZI előtt, hatékonyabb

🧰 7. Jelátvitel típusai
Alapsáv (baseband): nyers digitális jel

Szélessáv (broadband): modulált jel (AM/FM/PM)

🧪 8. Moduláció típusok
Moduláció Jellemző
AM Amplitúdó változik
FM Frekvencia változik
PM Fázis változik

🧮 9. Multiplexálási módszerek
Módszer Rövidítés Jellemző
Térbeli SDM külön vezeték/antenna
Frekvencia FDM eltérő frekvenciák
Időbeli TDM időszeletek, szinkron szükséges
Hullámhossz WDM optikai (pl. színes lézerek)
Kód CDMA egyedi kód sorozat minden állomásnak

💡 10. CDMA – Kódosztásos Többszörös Hozzáférés
Minden állomás saját chip-kóddal sugároz

Üzenet = chip-sorozat × bit

Vevő dekódolja ismert chip alapján

Ortogonális chipekkel működik → IS-95 mobil hálózat alapja

🤔 Tipikus vizsgakérdések:
Mi a fizikai réteg szerepe?

Milyen kódolási technikák vannak?

Melyek a fő átviteli közegek?

Hasonlítsd össze NRZ, Manchester és NRZI kódokat!

Magyarázd el CDMA működését egy példán!
