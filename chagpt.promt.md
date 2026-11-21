# Projekt: BMS & IT/OT – 12 hónapos szakmai fejlődési dashboard

> **Állapot (2026. 11. 21.):** megvalósítva a csr-appban → `html/bms_itot_12honap.html` (vanilla HTML + Firebase, nem React). A javított, élő tananyag ott van (`program-data` JSON-blokk); ez a fájl az eredeti prompt, nem frissül tovább. A döntések: `bms_it_ot_beszelgetes_reszletes_osszefoglalo.md`, 9. szakasz.

## 1. A projekt célja

Készíts egy modern, letisztult, könnyen használható személyes tanulási dashboardot, amellyel egy 12 hónapos szakmai fejlődési programot tudok követni.

A célom, hogy a jelenlegi backend fejlesztői munkámból fokozatosan egy BMS Systems Engineer / BMS Architect irányba fejlődjek, miközben megszerzem az ehhez szükséges IT/OT infrastruktúra-, hálózati és kiberbiztonsági ismereteket is.

Nem szeretnék általános backend fejlesztő maradni. A BMS és az épületautomatizálási rendszerek érdekelnek, különösen a teljes rendszerek megtervezése, felépítése, integrációja és hibakeresése.

Az IT/OT tudást azért szeretném elsajátítani, hogy ne csak a BMS-oldali integrációt értsem, hanem a teljes infrastruktúrát is átlássam a kontrollerektől a hálózaton és szervereken keresztül egészen a felhasználói felületig.

A program legyen fokozatos, gyakorlatias, és ne követeljen napi többórás tanulást.

**Tervezett tanulási idő: heti 5–7 óra.**

**Időtartam: 12 hónap, összesen 48 hét.**

A program ne legyen túl intenzív. A cél a mély megértés, nem a gyors végighaladás.

---

# 2. Szakmai hátterem – ezt vedd figyelembe a tananyag összeállításánál

Jelenleg egy kisebb cégnél dolgozom backend fejlesztőként, de a munkám egyre inkább BMS és ipari kommunikáció irányba tolódik.

A cég körülbelül 13 főből áll, így nincs minden szakterületre külön szakember.

Jelenlegi tapasztalataim:

- Backend fejlesztés.
- Python.
- BACnet.
- Modbus.
- OPC UA alapú integrációk tanulása.
- PROFINET rendszerek adatainak integrációja.
- Siemens kontrollerek.
- Adatpontok feldolgozása és integrációja.
- Szerveroldali kommunikáció.
- Windows Server és Windows környezet.
- Hibakeresés kommunikációs problémáknál.
- Windows Task Scheduler.
- BACpypes3 és Python asyncio.

Valós munkaproblémákkal is találkozom.

Például:
- BACnet Explorerből elérem az eszközt, Pythonból viszont nem.
- BBMD-beállítások és IP-kommunikáció.
- Modbus adatpontok integrációja.
- PROFINET esetében szimbolikus és abszolút címzés közötti különbségek.
- Hálózati útválasztási problémák.
- Több hálózati interfésszel rendelkező szerverek.
- VPN és tűzfal okozta kommunikációs problémák.

A hálózati infrastruktúrát és a tűzfalakat jelenleg külsős cégek kezelik.

Ezért különösen fontos, hogy megtanuljam értelmezni:
- A hálózati topológiákat.
- A rendszerarchitektúrákat.
- Az IP-címzési terveket.
- A VLAN-okat.
- A routingot.
- A tűzfalak működését.
- A szerverek és kontrollerek közötti kommunikációt.

Szeretném, ha a tananyag a már meglévő tapasztalataimra építene, nem pedig teljesen kezdőként kezelne.

---

# 3. A 12 hónapos tanulási program

A következő tematikát építsd be a dashboardba.

Minden hónap legyen külön megnyitható, azon belül pedig legyen négy hét.

Minden héthez tartozzon:
1. Heti tanulási cél.
2. Elméleti tananyag.
3. Konkrét tanulási témák.
4. Gyakorlati feladat.
5. Munkahelyi alkalmazási lehetőség.
6. Heti eredmény, amit el kell érnem.
7. Önellenőrző kérdések.

## 1. HÓNAP – BMS rendszerek és rendszerarchitektúra megértése

**Cél:** Megérteni, hogyan épül fel egy teljes BMS-rendszer.

1. hét – A BMS rendszerek felépítése
- Mi az a BMS?
- Mi a különbség a BMS, BAS, SCADA és EMS között?
- Milyen komponensekből áll egy épületautomatizálási rendszer?
- PLC-k, DDC-k, kontrollerek, szerverek és felhasználói felületek szerepe.
- Field level, automation level, management level.

Gyakorlat: Rajzolj fel egy egyszerű BMS architektúrát.

2. hét – Rendszerkomponensek és kommunikáció
- Siemens kontrollerek szerepe.
- I/O modulok.
- Érzékelők és beavatkozók.
- BMS szerverek.
- Gateway-ek.
- Kommunikációs protokollok.

Gyakorlat: Készíts egy ábrát arról, hogyan jut el egy hőmérséklet-érzékelő adata a BMS felületére.

3. hét – Rendszerarchitektúra és topológia
- Centralizált és decentralizált rendszerek.
- Client-server architektúra.
- Redundancia.
- Single point of failure.
- Rendszerbővítés.
- Skálázhatóság.

Gyakorlat: Készíts egy saját BMS rendszertervet.

4. hét – Valós projektek elemzése
- Munkahelyi rendszerrajzok értelmezése.
- Hálózati és automatizálási rajzok megkülönböztetése.
- Rendszerkomponensek azonosítása.
- Hiányzó információk összegyűjtése.

Havi eredmény: Egy teljes, saját BMS architektúra rajz.

## 2. HÓNAP – Hálózati alapok és IP-címzés

**Cél:** Megérteni az IP-alapú kommunikáció működését.

1. hét – TCP/IP alapok
- OSI modell.
- TCP és UDP.
- MAC és IP cím.
- Portok.
- DNS.
- DHCP.
- ARP.

Gyakorlat: Wireshark telepítése és egyszerű hálózati forgalom vizsgálata.

2. hét – IP-címzés és subnetting
- IPv4.
- Subnet mask.
- CIDR.
- Default gateway.
- Private és public IP.
- Hálózati tartományok.

Gyakorlat: Készíts egy IP-címzési tervet egy kisebb BMS-rendszerhez.

3. hét – Switching és VLAN
- Switch működése.
- Managed és unmanaged switch.
- VLAN.
- Access és trunk port.
- Broadcast domain.
- MAC address table.

Gyakorlat: Packet Tracerben készíts három külön VLAN-ból álló hálózatot.

4. hét – Hálózati hibakeresés
- Ping.
- Traceroute.
- Ipconfig.
- Nslookup.
- Netstat.
- Route print.
- ARP table.

Gyakorlat: Szimulálj egy hibás hálózati kapcsolatot, majd keresd meg az okát.

Havi eredmény: Egy működőképes, dokumentált IP- és VLAN-terv.

## 3. HÓNAP – Routing, tűzfalak és hálózati szegmentáció

**Cél:** Megérteni, hogyan kommunikálnak egymással az elkülönített hálózatok.

1. hét – Routing alapok
- Router működése.
- Routing table.
- Static routing.
- Default route.
- Inter-VLAN routing.

2. hét – Tűzfalak
- Firewall működése.
- Stateful és stateless firewall.
- Inbound és outbound szabályok.
- TCP és UDP portok.
- Allow és deny szabályok.

3. hét – IT és OT hálózatok szétválasztása
- IT/OT különbségek.
- Hálózati szegmentáció.
- DMZ.
- OT hálózatok védelme.
- Purdue Enterprise Reference Architecture alapjai.

4. hét – BMS hálózati tervezés
- BMS szerverek és kontrollerek hálózati kapcsolata.
- VLAN-ok kialakítása.
- Kommunikációs szabályok.
- Tűzfalszabályok dokumentálása.

Gyakorlat: Tervezz egy IT és OT szegmensekre bontott BMS hálózatot.

Havi eredmény: Egy hálózati topológia, VLAN-terv és kommunikációs mátrix.

## 4. HÓNAP – Wireshark és hálózati hibakeresés

**Cél:** Megtanulni, hogyan vizsgáljam a tényleges hálózati kommunikációt.

1. hét – Wireshark alapok
- Packet capture.
- Ethernet frame.
- IP packet.
- TCP és UDP.
- Display filter.

2. hét – TCP kommunikáció
- TCP handshake.
- SYN, ACK, FIN, RST.
- Portok és socketek.
- Connection timeout.

3. hét – UDP és ipari protokollok vizsgálata
- UDP működése.
- Broadcast és multicast.
- BACnet/IP alapú csomagok.
- Modbus TCP kommunikáció.

4. hét – Valós hibák elemzése
- Miért nem jön létre kapcsolat?
- Tűzfalblokkolás.
- Rossz IP-cím.
- Hibás port.
- Routing probléma.
- Timeout és sikertelen kommunikáció.

Gyakorlat: Készíts legalább három hibakeresési esettanulmányt.

Havi eredmény: Saját Wireshark hibakeresési jegyzetgyűjtemény.

## 5. HÓNAP – Modbus mélyebb megértése

**Cél:** A Modbus kommunikáció és adatpontok működésének megértése.

1. hét – Modbus alapok
- Modbus TCP.
- Modbus RTU.
- Master és Slave / Client és Server.
- Registerek.
- Coil és Discrete Input.

2. hét – Adatcímzés
- Holding Register.
- Input Register.
- Register offset.
- Function Code.
- 0-based és 1-based címzés.

3. hét – Adatértelmezés
- UINT16.
- INT16.
- FLOAT32.
- Byte order.
- Word order.
- Scaling.

4. hét – Gyakorlati integráció
- Modbus kliens készítése Pythonban.
- Adatok olvasása.
- Hibás címzés vizsgálata.
- Timeout kezelése.

Havi eredmény: Egy dokumentált Modbus kommunikációs tesztprojekt.

## 6. HÓNAP – BACnet mélyebb megértése

**Cél:** A BACnet architektúrájának és hálózati működésének megértése.

1. hét – BACnet alapok
- BACnet architektúra.
- BACnet/IP.
- BACnet MS/TP.
- Device ID.
- Object és Property.

2. hét – BACnet kommunikáció
- Who-Is.
- I-Am.
- ReadProperty.
- WriteProperty.
- Broadcast.
- Unicast.

3. hét – BACnet hálózatok
- BBMD.
- Foreign Device.
- Broadcast Distribution Table.
- BACnet hálózatok összekapcsolása.
- IP és UDP 47808.

4. hét – Hibakeresés és integráció
- BACpypes3.
- Python asyncio.
- Kommunikációs problémák.
- Wireshark vizsgálat.
- BBMD konfigurációs hibák.

Havi eredmény: Egy működő BACnet tesztkörnyezet és dokumentáció.

## 7. HÓNAP – OPC UA

**Cél:** Megérteni az OPC UA működését és biztonsági lehetőségeit.

1. hét – OPC UA architektúra
- Client-server.
- Server endpoint.
- Node és Namespace.
- Address Space.
- Information Model.

2. hét – OPC UA kommunikáció
- Read.
- Write.
- Subscription.
- Browse.
- Data monitoring.

3. hét – OPC UA biztonság
- Certificate.
- Authentication.
- Encryption.
- Security Policy.
- Secure Channel.

4. hét – Gyakorlati integráció
- OPC UA szerver szimulálása.
- Python kliens készítése.
- Adatok olvasása.
- Tanúsítványkezelés.

Havi eredmény: Működő OPC UA tesztprojekt dokumentációval.

## 8. HÓNAP – PROFINET és ipari kommunikáció

**Cél:** Megérteni az ipari Ethernet és PROFINET működését.

1. hét – PROFINET alapok
- PROFINET architektúra.
- IO Controller.
- IO Device.
- IO Supervisor.
- Real-time kommunikáció.

2. hét – Címzés és adatpontok
- IP-címzés.
- MAC-cím.
- Szimbolikus címzés.
- Abszolút címzés.
- PLC változók.
- I/O adatok.

3. hét – PLC és kommunikáció
- Siemens PLC alapok.
- PROFINET eszközök.
- GSDML.
- PLC adatblokkok.
- Adatkapcsolatok.

4. hét – Hibakeresés
- Kommunikációs problémák.
- Eszközazonosítás.
- Hibás címzés.
- Hálózati problémák.
- Diagnosztika.

Havi eredmény: Egy PROFINET kommunikációs architektúra és adatpont-dokumentáció.

## 9. HÓNAP – Szerverek és infrastruktúra

**Cél:** Megérteni, hogyan épül fel a BMS mögötti szerverinfrastruktúra.

1. hét – Szerver alapok
- Windows Server.
- Linux alapok.
- Server roles.
- Service management.
- Remote administration.

2. hét – Virtualizáció
- Hyper-V.
- VMware alapok.
- Virtual machine.
- Virtual switch.
- Virtuális hálózatok.

3. hét – BMS szerverarchitektúra
- Application server.
- Database server.
- Web server.
- Client-server kommunikáció.
- Adatbázis-kapcsolatok.

4. hét – Üzemeltetés
- Monitoring.
- Logging.
- Backup.
- Redundancia.
- Disaster recovery.

Havi eredmény: Egy dokumentált BMS szerverarchitektúra.

## 10. HÓNAP – IT/OT biztonság és rendszertervezés

**Cél:** Megérteni a biztonságos BMS/OT rendszerek tervezését.

1. hét – IT/OT cybersecurity
- OT biztonsági alapelvek.
- CIA triad.
- Least privilege.
- Defense in depth.
- IEC 62443 bevezetés.

2. hét – Hálózati biztonság
- Firewall rules.
- VLAN isolation.
- DMZ.
- VPN.
- Remote access.
- Secure communication.

3. hét – BMS biztonsági tervezés
- Kontrollerek védelme.
- BMS szerverek védelme.
- Hozzáférés-kezelés.
- Tanúsítványok.
- Naplózás.

4. hét – Biztonsági architektúra
- Kockázatelemzés.
- Hálózati zónák.
- Kommunikációs szabályok.
- Biztonsági dokumentáció.

Havi eredmény: Egy biztonsági koncepció egy saját BMS-rendszerhez.

## 11. HÓNAP – Teljes rendszerarchitektúra tervezése

**Cél:** Az eddig megszerzett tudás összekapcsolása.

1. hét – Követelmények és rendszertervezés
- Funkcionális követelmények.
- Nem funkcionális követelmények.
- Rendszerhatárok.
- Kapacitástervezés.
- Bővíthetőség.

2. hét – Hálózati és szerverarchitektúra
- Teljes hálózati topológia.
- IP-terv.
- VLAN-terv.
- Routing.
- Firewall.
- Szerverelhelyezés.

3. hét – Kommunikációs architektúra
- BACnet.
- Modbus.
- OPC UA.
- PROFINET.
- Gateway-ek.
- Adatáramlás.

4. hét – Dokumentáció és tervellenőrzés
- Hálózati rajzok.
- Rendszerarchitektúra.
- IP-címzési táblázat.
- Kommunikációs mátrix.
- Eszközlista.
- Hibakeresési terv.

Havi eredmény: Egy teljes BMS rendszerterv első változata.

## 12. HÓNAP – Önálló projekt és összefoglalás

**Cél:** Egy teljes rendszer megtervezése az eddig megszerzett tudás alapján.

1. hét – Projekt követelményei
- Egy kisebb irodaház vagy kereskedelmi épület kiválasztása.
- Rendszerkövetelmények.
- Kontrollerek.
- Szerverek.
- Adatpontok.
- Kommunikációs igények.

2. hét – Architektúra
- BMS topológia.
- IT/OT hálózat.
- IP-címzési terv.
- VLAN-ok.
- Szerverstruktúra.

3. hét – Kommunikáció és biztonság
- BACnet vagy Modbus.
- OPC UA.
- Hálózati kommunikáció.
- Tűzfalszabályok.
- Biztonsági zónák.

4. hét – Dokumentáció és bemutatás
- Teljes rendszerarchitektúra.
- Hálózati diagram.
- Kommunikációs mátrix.
- Eszközlista.
- Biztonsági koncepció.
- Hibakeresési dokumentáció.
- Projektbemutató.

Havi eredmény: Egy saját, portfólióban is bemutatható BMS/IT/OT rendszerterv.

---

# 4. A dashboard felépítése

A felület legyen modern, professzionális, technikai jellegű, de ne legyen túlzsúfolt.

Szeretnék egy áttekinthető főoldalt.

## Főoldal – Dashboard

Jelenjen meg:

- 12 hónapos program előrehaladása.
- Teljesített hetek száma.
- Hátralévő hetek száma.
- Aktuális hónap.
- Aktuális hét.
- Teljesített tanulási feladatok.
- Heti célkitűzés.
- Következő feladat.
- Tanulással töltött idő.

Legyen egy nagy, jól látható progress bar.

Például:

12 hónap teljesítése: 0%

Teljesített hetek: 0 / 48

## Havi naptár

Legyen egy 12 hónapos áttekintő nézet.

Minden hónap külön kártyaként jelenjen meg.

A kártyán szerepeljen:
- Hónap neve.
- Fő tanulási téma.
- Hetek száma.
- Teljesítési százalék.
- Havi státusz.

A hónapra kattintva nyíljon meg a négyhetes részletes tanulási terv.

## Heti tanulási nézet

Minden hét külön oldalon vagy részletes panelen jelenjen meg.

Legyen rajta:

- A hét témája.
- A heti cél.
- Elméleti tananyag.
- Gyakorlati feladatok.
- Munkahelyi alkalmazás.
- Heti eredmény.
- Önellenőrző kérdések.

Minden feladat mellett legyen checkbox.

Ha egy feladatot befejeztem, tudjam kipipálni.

A hét akkor legyen teljesített, ha minden kötelező feladatot elvégeztem.

## Heti naptár és időbeosztás

A heti 5–7 órás tanulást lehessen felosztani.

Alapértelmezett javaslat:

- Hétfő: 1 óra elmélet.
- Kedd: 1 óra tananyag.
- Szerda: pihenő vagy ismétlés.
- Csütörtök: 1 óra gyakorlás.
- Péntek: 1 óra gyakorlás.
- Szombat: 1–2 óra projekt vagy összefoglalás.
- Vasárnap: opcionális ismétlés.

Ezt lehessen módosítani.

Legyen lehetőség egy-egy tanulási alkalomhoz időpontot és időtartamot rendelni.

## Jegyzetek

Minden héthez tartozzon saját jegyzetmező.

Szeretném feljegyezni:
- Mit tanultam.
- Mit értettem meg.
- Mi nem világos.
- Milyen kérdéseim vannak.
- Milyen munkahelyi problémával találkoztam.
- Milyen megoldást találtam.

Legyen lehetőség hosszabb jegyzetek mentésére.

## Munkahelyi tapasztalatok

Külön menüpontot szeretnék a valós munkahelyi problémák dokumentálására.

Például:
- BACnet kommunikációs hiba.
- Modbus címzési probléma.
- PROFINET szimbolikus és abszolút címzés.
- Routing probléma.
- Firewall probléma.
- Szerverkommunikáció.

Minden bejegyzéshez tartozzon:
- Probléma leírása.
- Érintett technológia.
- Hiba oka.
- Megoldás.
- Tanulság.

## Havi értékelés

Minden hónap végén jelenjen meg egy havi értékelő oldal.

Kérdések:
1. Mit tanultam ebben a hónapban?
2. Melyik témát értem a legjobban?
3. Mi okozta a legnagyobb nehézséget?
4. Mit tudtam alkalmazni a munkámban?
5. Mit kell még gyakorolnom?
6. Készen állok a következő hónapra?

A következő hónapra akkor is lehessen továbblépni, ha nem teljesítettem minden feladatot.

---

# 5. Technikai elvárások

A meglévő projekt struktúráját először vizsgáld meg, és ahhoz igazítsd a megvalósítást.

Ha nincs még projekt, használj modern frontend megoldást.

Preferált technológiák:
- React.
- TypeScript.
- Tailwind CSS.
- Lucide ikonok.

A megoldás legyen egyszerűen futtatható és később bővíthető.

Adattárolás:
- Első verzióban használhatsz localStorage-t.
- A teljesített feladatok maradjanak meg újratöltés után is.
- A jegyzetek és időbeosztások is mentődjenek.
- Legyen lehetőség az adatok exportálására és importálására JSON formátumban.

Fontos:
- Ne legyen szükség backend szerverre az első verzióhoz.
- Ne legyen szükség felhasználói regisztrációra.
- Ne legyen szükség fizetős szolgáltatásokra.
- A felület legyen reszponzív.

---

# 6. Design és felhasználói élmény

Modern, letisztult technikai dashboardot szeretnék.

Inspiráció:
- Linear.
- Notion.
- Modern project management dashboardok.

Megjelenés:
- Sötét és világos mód.
- Áttekinthető oldalsó navigáció.
- Kártyás elrendezés.
- Progress barok.
- Naptár.
- Diagramok.
- Jól elkülönített tanulási modulok.

Ne legyen túl sok szín vagy animáció.

A felület teljes egészében magyar nyelvű legyen.

A technikai kifejezéseket viszont hagyd meg angolul is, például:
- Network Architecture.
- Firewall.
- Routing.
- Switching.
- BMS.
- IT/OT.
- OPC UA.

---

# 7. Fontos működési szabályok

1. A 48 hetes tananyag legyen előre betöltve.
2. Ne csak címeket jeleníts meg, hanem minden hétnek legyen konkrét tanulási tartalma.
3. A feladatok teljesítését lehessen egyenként követni.
4. Az előrehaladás automatikusan számolódjon.
5. A jegyzetek ne vesszenek el.
6. A befejezetlen heteket később is folytathassam.
7. Ne kényszeríts merev naptári határidőkre.
8. A tanulási tervet később szerkeszthetővé kell tenni.
9. Minden hónap végén legyen egy konkrét kézzelfogható eredmény.
10. A program a BMS rendszertervezést helyezze előtérbe, de folyamatosan építse mellé az IT/OT hálózati és infrastruktúra-tudást.

A tananyagban szereplő gyártóspecifikus funkciókat, protokollrészleteket és szabványokat mindig ellenőrizhető dokumentációhoz igazítsd. Ne találj ki technikai specifikációkat.

---

# 8. A végső cél

A 12 hónap végére szeretném, ha képes lennék:

- Megérteni egy teljes BMS-rendszer architektúráját.
- Értelmezni a hálózati topológiákat.
- IP-címzési és VLAN-terveket készíteni.
- Megérteni a routing és firewall szabályok szerepét.
- Átlátni a BACnet, Modbus, OPC UA és PROFINET működését.
- Megérteni a szerverinfrastruktúra felépítését.
- Felismerni az IT/OT biztonsági kockázatokat.
- Részt venni egy teljes BMS-rendszer megtervezésében.
- Önállóan elkészíteni egy kisebb BMS-rendszer architektúráját és dokumentációját.

**A legfontosabb: ne egy egyszerű teendőlistát készíts, hanem egy olyan személyes szakmai fejlődési platformot, amelyet 12 hónapon keresztül nap mint nap használhatok.**

Először készítsd el a működő alapverziót a teljes 48 hetes tananyaggal, majd ellenőrizd, hogy a navigáció, a feladatok kipipálása, a mentés és a haladáskövetés megfelelően működik-e.