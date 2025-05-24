📚 Telekommunikációs Hálózatok – Előadás 1 Összefoglaló
🌐 Az Internet mérete és szerepe
2023-ra ~30 milliárd eszköz kapcsolódott az internetre.

Napi internetes adatforgalom ~13 exabájt.

A teljes IP forgalom 82%-a videó.

🛑 Internet veszélyei
Politikai lekapcsolások, PRISM program (megfigyelés).

Netsemlegesség kérdése: ISP lassíthat-e bizonyos forgalmat?

Netflix vs. ISP: ki fizet az adatforgalomért?

💥 Sérülékenység példák
BGP szivárgás → forgalom rossz helyre megy.

Emberi hibák → a kiesések 50–80%-át okozzák.

🧠 A tárgy fő kérdései
Címzés – hogyan címezhetők eszközök?

Rétegek – hogyan kezeljük a komplexitást?

Forgalomirányítás – hogyan jutunk el A-ból B-be?

Megbízhatóság – hogyan biztosítsunk megbízható átvitelt?

Erőforrás megosztás – hogyan osszuk el a sávszélességet?

🧱 Hálózati építőelemek
Végpontok: mobil, PC, szerver, okoseszközök.

Switchek és routerek: adatirányítás.

Linkek: réz, optikai, vezeték nélküli.

🧮 Hálózati sávszélesség
Mértékegység: bps (bit per second), pl. Mbps, Gbps, Tbps.

📡 Hozzáférési technológiák
DSL (ADSL) – telefonvonal, aszimmetrikus.

KábelTV (CATV) – közös közeg, aszimmetrikus.

Ethernet (LAN) – leggyakoribb helyi hálózat.

🕸 Topológia és erőforrásmegosztás
Hibatolerancia = több útvonal

Teljes összeköttetés nem praktikus → switchelt hálózatok

🔄 Multiplexálás típusai
Előre foglalás: garantált erőforrás, de pazarló.

Igény szerinti: hatékonyabb, de változó teljesítmény.

🔁 Kapcsolás típusok
Típus Példa Jellemzők
Áramkörkapcsolt Telefon Előre foglalás, kiszámítható, de nem hatékony
Csomagkapcsolt Internet Igény szerinti, hatékony, de nem kiszámítható

🏛 Internet felépítése
ISP (Access, Tier-3, Tier-2, Tier-1) – hierarchikus.

Peering – közvetlen kapcsolatok a költségcsökkentésért.

IXP (Internet Exchange Point) – hálózatok csatlakozása.

📜 Történelem röviden
1969: ARPANET elindul – az első üzenet „LO”

1974: TCP/IP alapjai lefektetve (Cerf & Kahn)

1983: DNS bevezetése

1989: Web születése (Tim Berners-Lee)

1990-es évek: Google, keresők, modern internet

<!-- 2 -->

📚 Telekommunikációs Hálózatok – Előadás 2 Összefoglaló
📡 Kommunikáció lényege
Az Internet célja: különböző gépeken futó folyamatok adatot cserélhessenek.

Ez protokollok segítségével történik.

A protokoll: szabályrendszer, ami meghatározza a kommunikáció menetét.

🔁 Modularitás
Nagy rendszerek nem működhetnek „spagetti kód” alapján.

Megoldás: Rétegek bevezetése – modularitás + absztrakció

Minden réteg szolgáltatást nyújt a fölötte lévőnek, az alatta lévő használatával.

📦 Rétegmodellek
🌍 TCP/IP modell (RFC 1122) – 4 réteg
Alkalmazási réteg – HTTP, FTP, DNS stb.

Szállítási réteg – TCP (megbízható), UDP (nem megbízható)

Hálózati réteg – IP, útvonalválasztás

Kapcsolati réteg – Ethernet, WiFi, fizikai kapcsolat

🌐 OSI modell – 7 réteg
Fizikai réteg – bit átvitel (kábel, rádió, stb.)

Adatkapcsolati réteg – keretezés, MAC, hibakezelés

Hálózati réteg – IP, routing

Szállítási réteg – TCP/UDP, portok

Ülés réteg – kapcsolat kezelése, szinkronizálás (ritkán van külön implementálva)

Megjelenítési réteg – adatformátum konverzió (ASCII, Unicode, stb.)

Alkalmazási réteg – konkrét hálózati alkalmazások

📌 Fontos: A TCP/IP és OSI rétegmodell összevonható: gyakorlatban a 7 rétegből inkább 5 működik.

🧱 Protokoll adategységek (PDU-k)
Alkalmazás → üzenet

Szállítási → szegmens

Hálózati → csomag (packet)

Kapcsolati → keret (frame)

Fizikai → bitek

🌐 Hálózati eszközök réteg szerint
Hoszt: minden réteget implementál (L1–L5)

Router: L3-ig működik (hálózati rétegig)

Switch: csak L2 (adatkapcsolati réteg)

⏱ Hálózati teljesítmény jellemzői

1. Késleltetés (delay) =
   Átviteli késleltetés

Terjedési késleltetés

Feldolgozási idő

Sorban állási idő

🧠 Képletek:

Átviteli késleltetés = méret [bit] / sávszélesség [bps]

Terjedési késleltetés = távolság / terjedési sebesség (pl. fénysebesség rostban)

2. Sorban állási késleltetés
   Függ: beérkezési ráta, link sávszélessége, forgalom löketszerűsége

Traffic intensity = La / R

Ha >1 → sor végtelen nő

Ha <=1 → késleltetés változó

3. Veszteség (loss)
   Sorok nem végtelenek → túlterhelésnél csomageldobás

4. Áteresztőképesség (throughput)
   Átlagos = adat méret / átvitel ideje

Bottleneck link határozza meg

✅ Extra tipp:
Encapsulation (beágyazás) – minden réteg hozzáadja a saját fejlécét az adatcsomaghoz.
Pl.: HTTP → TCP → IP → Ethernet (header-ek egymásba ágyazva)

<!-- 3 -->
📚 Telekommunikációs Hálózatok – Előadás 3 Összefoglaló
⚡ Fizikai réteg szerepe
Szolgáltatás: bitek átvitele két eszköz között.

Protokoll: jelátvitel módja (pl. feszültségszintek, időzítés).

Példák: koaxiális kábel, optikai kábel, rádiófrekvencia.

🎯 Alapfogalmak
Digitális gépek 0 és 1 jelekkel dolgoznak.

Analóg világ amplitúdóval, frekvenciával.

ASCII karakter (pl. „b”) több bitből áll → feszültséggel átvitel.

🎶 Jelátvitel és torzulás
Fourier-sor segítségével digitális jel leírható.

Valós közegekben:

frekvenciafüggő elnyelődés

fáziseltolódás

zaj (pl. hő, más rendszerek zavarása)

🧠 Szimbólum és bit különbsége
Egy szimbólum több bitet jelenthet.

Baud = szimbólum/sec, bps = bit/sec

Pl. 16 szimbólum = 4 bit → 600 Baud = 2400 bps

🔌 Vezetékes közegek
Sodort érpár: UTP/STP, telefonrendszerekben

Koax kábel: gyorsabb, távolabbra

Fényvezető szál: impulzus = 1, nincs = 0; nagy távolság, magas sávszélesség

📡 Vezeték nélküli közeg
Rádiófrekvenciás: nagy távolság, egyszerű

Mikrohullám: egyenes vonalban, olcsó

Infravörös/Látható fény: kistávolság, akadály érzékeny

Elektromágneses spektrum:

VLF → SHF, pl. TV, mobil, műhold

🛰 Műholdas kommunikáció
Geoszinkron (35 800 km): 270 ms késés, 3 műhold

Közepes pályás: 35–85 ms, 10 műhold

Alacsony pályás: 1–7 ms, 50 műhold

🔁 Digitális jel kódolások
NRZ: 1 = magas, 0 = alacsony

Probléma: sok egymás utáni 0/1 szinkronhibát okoz

Manchester: mindig vált, 1 = magas→alacsony, 0 = alacsony→magas

Szinkron megoldás, de fele sávszélességet használ

NRZI: 1 = váltás, 0 = nem vált

📌 Ethernet példák:

10BASE-TX: Manchester

100BASE-TX: 4B/5B + NRZI

Gigabit Ethernet: 8B/10B kódolás

📶 Átviteli technikák
🎚 Baseband vs Broadband
Baseband: közvetlen feszültségátvitel

Broadband: modulációval több jel → több frekvencia

📊 Multiplexálási módszerek
TDM – időbeli

FDM – frekvencia

WDM – hullámhossz (optika)

SDM – térbeli

CDM – kód alapú (mobilhálózat, IS-95)

🔢 CDMA működés alapjai
Töredékkód (chip sequence) alapján minden állomás saját kódot használ

A vevő az ismert chip kóddal tudja visszafejteni a jelet

Több állomás egyszerre küldhet a teljes spektrumon

✅ Tipp: Kódolások + multiplexálási technikák → gyakran jönnek MC kérdésben!