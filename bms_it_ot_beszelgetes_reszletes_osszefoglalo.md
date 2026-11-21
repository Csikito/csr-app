# BMS és IT/OT karriertervezés -- beszélgetési összefoglaló

**Dátum:** 2026. november\
**Téma:** A jelenlegi backend fejlesztői munkából BMS-központú
rendszermérnöki és rendszertervezési irányba fejlődés, IT/OT és hálózati
tudással kiegészítve.

> Ez a dokumentum a beszélgetés tartalmát időrendben, részletesen és
> szerkesztett formában rögzíti. A hangalapú üzeneteknél a
> félrehallásokat és ismétléseket a jelentés megőrzésével javítottam.
> Nem szó szerinti hangfelvétel-átirat.

------------------------------------------------------------------------

## 1. Kiindulópont: milyen szakmai háttérrel rendelkezel?

Elmondtad, hogy jelenleg backend fejlesztőként dolgozol egy kis
vállalkozásnál, de hosszabb távon nem szeretnél általános fejlesztő
maradni. A BMS és az épületautomatizálás sokkal jobban érdekel, és ezen
a területen szeretnél elmélyülni.

A cégnél körülbelül 13 ember dolgozik. A csapat felépítése nagyjából a
következő:

-   3--4 fejlesztő;
-   egy IT-t menedzselő vezető;
-   1--2 automatizálási szakember;
-   egy villamos szakember;
-   ajánlatok beszerzésével foglalkozó munkatárs;
-   automatizálási tervezéssel foglalkozó kolléga;
-   a cégvezető, aki a leadek és a kereskedelmi terület irányításában is
    részt vesz;
-   a kereskedelmi területen további egy munkatárs.

A kis létszám miatt sok szakterületből csak egy-egy ember van, miközben
a fejlesztői és automatizálási csapat valamivel nagyobb.

### A jelenlegi munkád

A munkád backend fejlesztésből indult, de egyre több BMS-integrációs
feladatot végzel. Jellemzően adatpontlistákat kapsz, és az a feladatod,
hogy az adatokat a megfelelő kommunikációs protokollon keresztül elérd
és integráld.

A munkádhoz kapcsolódó technológiák és területek:

-   Python és backend fejlesztés;
-   BACnet;
-   Modbus;
-   OPC UA -- ezt mostanában kezdted jobban megismerni;
-   PROFINET;
-   Siemens kontrollerek;
-   adatpontok integrációja és értelmezése;
-   szerveroldali kommunikáció;
-   kommunikációs hibák feltárása.

Korábbi konkrét technikai témáink között szerepelt a BACpypes3, az
asyncio, a BBMD, a BACnet Explorer és a Python közötti kommunikációs
eltérés, a Modbus-adatpontok, a PROFINET szimbolikus és abszolút
címzése, valamint a több hálózati interfésszel rendelkező szerverek
útválasztási problémái.

Azt is elmondtad, hogy a hálózati infrastruktúrát -- például a LAN-t, a
tűzfalakat és bizonyos hálózati beállításokat -- jelenleg külsős cégek
kezelik. Te általában megkapod a kontrollerek IP-címeit és az
adatpontlistát, majd a BMS-oldali integrációt végzed.

Ha nem sikerül kiolvasni egy adatot Modbuson, OPC UA-n vagy más
protokollon keresztül, utánajársz a problémának. Megpróbálod feltárni,
hogy nálatok, a külsős hálózatos cégnél, a vezérlőnél vagy a
kommunikációs beállításokban van-e az ok.

Különösen élvezed ezeket a hibakeresési helyzeteket. Többször
előfordult, hogy olyan problémával találkoztál, amelyre a cégen belül
sem volt azonnal kész válasz. Ilyenkor te kezdted feltárni a működést,
és közösen tanultátok meg, hogyan kell kezelni az adott esetet.

Ezt nem feltétlenül hibának látod a cégnél: inkább olyan területnek,
amelyre korábban még nem voltatok felkészülve.

------------------------------------------------------------------------

## 2. Milyen szakmai irány érdekel?

Elmondtad, hogy nem egyszerűen a backend fejlesztést szeretnéd
folytatni. Sokkal jobban érdekel:

-   a BMS-rendszerek mélyebb megértése;
-   a teljes épületautomatizálási rendszer felépítése;
-   a rendszertervezés és az architektúra;
-   a kontrollerek, szerverek és hálózatok közötti kapcsolatok;
-   az ipari kommunikáció;
-   a hálózatok és a tűzfalak működése;
-   az IT és OT rendszerek összekapcsolása;
-   a hibakeresés és a teljes rendszer átlátása.

A célod az, hogy ne csak egy már megtervezett rendszerbe integrálj
adatpontokat, hanem idővel részt tudj venni abban is, hogy az egész
rendszer hogyan épüljön fel.

Például szeretnéd megérteni:

-   milyen szempontok alapján alakítanak ki egy BMS-hálózatot;
-   miért választanak egy adott hálózati topológiát;
-   hogyan kapcsolódnak a kontrollerek a szerverekhez;
-   milyen VLAN-okat és IP-tartományokat használnak;
-   hol helyezkednek el a tűzfalak;
-   milyen kommunikációs szabályokra van szükség;
-   hogyan választják szét az IT- és OT-hálózatokat;
-   hogyan lehet a rendszert biztonságosan és bővíthetően megtervezni.

### A cégen belüli lehetőség és korlát

A jelenlegi cégednél nincs feltétlenül olyan belső szakember, akitől a
teljes hálózati és IT/OT rendszertervezést közvetlenül megtanulhatnád. A
hálózati tervezés jelentős része külsős cégek feladata.

Ezért felmerült benned, hogy ezt a tudást valószínűleg önálló
tanulással, kurzusokkal és gyakorlati laborokkal kell megszerezned.

Arra jutottunk, hogy nem szükséges rögtön munkahelyet váltanod. A
jelenlegi cégednél is sokat fejlődhetsz, ha fokozatosan közelebb kerülsz
a tervezési folyamathoz.

Konkrét javaslat volt, hogy amikor egy külsős cég átad egy hálózati
tervet vagy topológiai rajzot, kérd el vagy kérd meg, hogy
megtekinthesd. Először csak próbáld értelmezni:

-   milyen eszközök szerepelnek rajta;
-   melyik eszköz mihez kapcsolódik;
-   hol vannak a hálózati szegmensek;
-   hogyan jut el az adat a kontrollertől a szerverig;
-   hol vannak a tűzfalak és az átjárók.

Nem kell elsőre mindent megértened. Írd fel a kérdéseidet, nézz utána
később, majd a következő projektben kérdezz célzottabban a külsős
szakemberektől.

------------------------------------------------------------------------

## 3. A három lehetséges karrierirány

Megvizsgáltuk, milyen irányokba fejlődhetnél tovább. Három lehetséges
szakmai profilt különítettünk el.

### A) BMS Systems Engineer

Ez áll legközelebb a jelenlegi érdeklődésedhez.

A fókusz a teljes épületautomatizálási rendszeren van:

-   BMS-rendszerek felépítése;
-   Siemens és más gyártók kontrollerei;
-   BACnet, Modbus, OPC UA;
-   adatpontok és integrációk;
-   BMS-szerverek;
-   grafikus felületek;
-   rendszerarchitektúra;
-   üzembe helyezés és hibakeresés;
-   épületgépészeti és automatizálási rendszerek összekapcsolása.

Egy ilyen szakember nem pusztán adatpontokat integrál, hanem átlátja a
teljes épületautomatizálási rendszert, és részt vesz annak
megtervezésében.

Lehetséges későbbi irányok: BMS Systems Engineer, BMS Design Engineer,
BMS Solution Architect vagy BMS Architect.

### B) IT/OT Systems Engineer

Ez szélesebb ipari infrastruktúra-irány.

A fókusz az informatikai és az ipari/automatizálási rendszerek közötti
kapcsolaton van:

-   ipari hálózatok;
-   routing és switching;
-   VLAN-ok;
-   tűzfalak;
-   szerverek;
-   biztonságos távoli hozzáférés;
-   OPC UA és más ipari protokollok;
-   OT-hálózati szegmentáció;
-   ipari kiberbiztonság;
-   IT/OT architektúra.

Ez a terület nem kizárólag épületautomatizálásban használható.
Gyártóüzemekben, energetikai rendszerekben és más ipari környezetekben
is releváns.

### C) Infrastructure / Network Engineer

Ez már általánosabb IT-infrastruktúra irány.

A főbb témák:

-   vállalati hálózatok;
-   routing és switching;
-   LAN és WAN;
-   VLAN-ok;
-   tűzfalak;
-   Windows Server és Linux;
-   virtualizáció;
-   szerverüzemeltetés;
-   monitoring;
-   backup;
-   vállalati kiberbiztonság.

Ez a profil kevésbé kötődik a BMS-hez és az ipari automatizáláshoz.
Cserébe szélesebb általános infrastruktúra-tudást ad.

### A három irány összehasonlítása

  ------------------------------------------------------------------------
  Szempont           BMS Systems       IT/OT Systems     Infrastructure /
                     Engineer          Engineer          Network Engineer
  ------------------ ----------------- ----------------- -----------------
  BMS                Nagyon erős       Kapcsolódó        Kevésbé jellemző
                     fókusz            terület           

  Ipari protokollok  Erős              Erős              Korlátozott

  Hálózatok          Közepes--erős     Erős              Nagyon erős

  Szerverek          Közepes           Erős              Nagyon erős

  Rendszertervezés   Nagyon erős       Nagyon erős       Erős

  IT/OT biztonság    Kapcsolódó        Nagyon erős       Általános
                                                         IT-biztonság
  ------------------------------------------------------------------------

------------------------------------------------------------------------

## 4. Melyik irány mellett döntöttünk?

A beszélgetés végére arra jutottunk, hogy számodra a BMS Systems
Engineer irány a legvonzóbb.

Nem szeretnéd elhagyni a BMS-t, mert maga az épületautomatizálás, a
kontrollerek, az integráció és a rendszertervezés érdekel.

Ugyanakkor nem szeretnéd túlságosan beszűkíteni a tudásodat egyetlen
gyártóra vagy iparágra.

Ezért a közösen kialakított stratégia:

**BMS-központú szakmai fejlődés, IT/OT hálózati és
infrastruktúra-tudással kiegészítve.**

A cél nem az, hogy általános hálózati mérnökké válj, és ne is az, hogy
kizárólag egyetlen BMS-terméket ismerj.

A cél az, hogy olyan szakember legyél, aki érti a BMS-rendszert, de a
mögötte lévő teljes informatikai és ipari infrastruktúrát is képes
átlátni.

A korábban javasolt tanulási hangsúlyok:

  Terület                              Hangsúly
  ---------------------------------- ----------
  Hálózatok és infrastruktúra               30%
  Rendszerarchitektúra és tervezés          30%
  Ipari kommunikáció                        20%
  Kiberbiztonság                            15%
  Szoftveres integráció                      5%

Ezek irányadó tanulási arányok, nem merev követelmények.

------------------------------------------------------------------------

## 5. A 12 hónapos tanulási program

A program célja, hogy a jelenlegi tudásodra építve fokozatosan eljuss a
teljes BMS-rendszerek tervezésének megértéséig.

**Tervezett tanulási idő: heti 5--7 óra.**

**Időtáv: 12 hónap, 48 hét.**

A hangsúly a mély megértésen és a gyakorlati alkalmazáson van, nem a
gyors haladáson.

### 1. hónap -- BMS-rendszerek és rendszerarchitektúra

1.  hét: BMS alapok, BAS, SCADA, EMS, field/automation/management level,
    rendszerkomponensek.

2.  hét: Kontrollerek, I/O modulok, érzékelők, beavatkozók, gateway-ek,
    szerverek és kommunikációs protokollok.

3.  hét: Centralizált és decentralizált rendszerek, client-server
    architektúra, redundancia, single point of failure, skálázhatóság.

4.  hét: Valós BMS-projektek és hálózati rajzok értelmezése.

**Havi eredmény:** egy saját, teljes BMS-architektúra rajz.

### 2. hónap -- Hálózati alapok és IP-címzés

1.  hét: OSI modell, TCP/IP, TCP, UDP, MAC és IP-cím, DNS, DHCP, ARP.

2.  hét: IPv4, subnet mask, CIDR, default gateway, private és public IP,
    IP-címzési terv.

3.  hét: Switching, managed és unmanaged switch, VLAN, access és trunk
    port, broadcast domain.

4.  hét: Ping, traceroute, ipconfig, nslookup, netstat, route print és
    alapvető hibakeresés.

**Havi eredmény:** egy dokumentált IP- és VLAN-terv.

### 3. hónap -- Routing, tűzfalak és hálózati szegmentáció

1.  hét: Router, routing table, static routing, default route,
    inter-VLAN routing.

2.  hét: Firewall működése, stateful és stateless firewall,
    inbound/outbound szabályok, TCP/UDP portok.

3.  hét: IT/OT hálózatok, szegmentáció, DMZ, Purdue-modell.

4.  hét: BMS hálózatok tervezése, kommunikációs szabályok és mátrixok.

**Havi eredmény:** IT/OT szegmensekre bontott BMS hálózati terv.

### 4. hónap -- Wireshark és hálózati hibakeresés

1.  hét: Packet capture, Ethernet frame, IP packet, TCP/UDP és display
    filter.

2.  hét: TCP handshake, SYN, ACK, FIN, RST, timeout és socketek.

3.  hét: UDP, broadcast, multicast, BACnet/IP és Modbus TCP csomagok.

4.  hét: Kommunikációs hibák, tűzfalblokkolás, hibás IP, routing és
    timeout elemzése.

**Havi eredmény:** legalább három dokumentált hibakeresési
esettanulmány.

### 5. hónap -- Modbus

1.  hét: Modbus TCP, Modbus RTU, Client/Server, Coil, Discrete Input és
    Register.

2.  hét: Holding Register, Input Register, Function Code, offset és
    címzési különbségek.

3.  hét: UINT16, INT16, FLOAT32, byte order, word order és scaling.

4.  hét: Python Modbus kliens, adatolvasás, címzési hibák és timeout
    kezelése.

**Havi eredmény:** dokumentált Modbus tesztprojekt.

### 6. hónap -- BACnet

1.  hét: BACnet architektúra, BACnet/IP, MS/TP, Device ID, Object és
    Property.

2.  hét: Who-Is, I-Am, ReadProperty, WriteProperty, broadcast és
    unicast.

3.  hét: BBMD, Foreign Device, BDT és BACnet hálózatok összekapcsolása.

4.  hét: BACpypes3, asyncio, Wireshark és BACnet hibakeresés.

**Havi eredmény:** működő BACnet tesztkörnyezet és dokumentáció.

### 7. hónap -- OPC UA

1.  hét: OPC UA architektúra, Client-Server, Endpoint, Node, Namespace
    és Address Space.

2.  hét: Read, Write, Subscription és Browse.

3.  hét: Certificate, Authentication, Encryption, Security Policy és
    Secure Channel.

4.  hét: OPC UA szerver szimulálása, Python kliens, adatolvasás és
    tanúsítványkezelés.

**Havi eredmény:** működő OPC UA tesztprojekt.

### 8. hónap -- PROFINET és ipari kommunikáció

1.  hét: PROFINET architektúra, IO Controller, IO Device és IO
    Supervisor.

2.  hét: IP- és MAC-címzés, szimbolikus és abszolút címzés, PLC-változók
    és I/O adatok.

3.  hét: Siemens PLC alapok, GSDML, adatblokkok és adatkapcsolatok.

4.  hét: Kommunikációs hibák, eszközazonosítás és diagnosztika.

**Havi eredmény:** PROFINET kommunikációs architektúra és
adatpont-dokumentáció.

### 9. hónap -- Szerverek és infrastruktúra

1.  hét: Windows Server, Linux alapok, server roles, service management
    és távoli adminisztráció.

2.  hét: Hyper-V, VMware, virtual machine és virtuális hálózatok.

3.  hét: BMS Application Server, Database Server, Web Server és
    client-server kommunikáció.

4.  hét: Monitoring, logging, backup, redundancia és disaster recovery.

**Havi eredmény:** dokumentált BMS szerverarchitektúra.

### 10. hónap -- IT/OT biztonság és rendszertervezés

1.  hét: OT cybersecurity, CIA triad, least privilege, defense in depth
    és IEC 62443.

2.  hét: Firewall, VLAN isolation, DMZ, VPN, remote access és secure
    communication.

3.  hét: Kontrollerek, BMS-szerverek, hozzáférések és tanúsítványok
    védelme.

4.  hét: Kockázatelemzés, hálózati zónák, kommunikációs szabályok és
    biztonsági dokumentáció.

**Havi eredmény:** biztonsági koncepció egy saját BMS-rendszerhez.

### 11. hónap -- Teljes rendszerarchitektúra tervezése

1.  hét: Funkcionális és nem funkcionális követelmények,
    rendszerhatárok, kapacitás és bővíthetőség.

2.  hét: Hálózati topológia, IP-terv, VLAN-terv, routing, firewall és
    szerverelhelyezés.

3.  hét: BACnet, Modbus, OPC UA, PROFINET, gateway-ek és adatáramlás.

4.  hét: Hálózati rajzok, kommunikációs mátrix, eszközlista és
    tervellenőrzés.

**Havi eredmény:** egy teljes BMS rendszerterv első változata.

### 12. hónap -- Önálló projekt

Egy kisebb irodaház vagy kereskedelmi épület teljes BMS-rendszerének
megtervezése.

1.  hét: Követelmények, kontrollerek, szerverek, adatpontok és
    kommunikációs igények.

2.  hét: BMS-topológia, IT/OT hálózat, IP-címzés, VLAN-ok és
    szerverstruktúra.

3.  hét: Kommunikációs protokollok, tűzfalszabályok és biztonsági zónák.

4.  hét: Teljes dokumentáció, hálózati diagram, kommunikációs mátrix,
    eszközlista, biztonsági koncepció és projektbemutató.

**Havi eredmény:** egy saját, portfólióban is bemutatható BMS/IT/OT
rendszerterv.

------------------------------------------------------------------------

## 6. Hogyan szeretnéd követni a tanulást?

Felmerült, hogy a 12 hónapos programhoz saját naptárt vagy dashboardot
készítesz Codex segítségével.

A cél egy személyes tanulási platform, ahol:

-   látható a 12 hónapos előrehaladás;
-   követhetők a 48 heti modulok;
-   kipipálhatók az elvégzett feladatok;
-   rögzíthető a tanulással töltött idő;
-   minden héthez tartozik saját jegyzet;
-   dokumentálhatók a munkahelyi technikai problémák;
-   minden hónap végén elvégezhető egy önértékelés;
-   láthatók a havi kézzelfogható eredmények.

### Tervezett heti időbeosztás

-   Hétfő: 1 óra elmélet.
-   Kedd: 1 óra tananyag.
-   Szerda: pihenő vagy ismétlés.
-   Csütörtök: 1 óra gyakorlás.
-   Péntek: 1 óra gyakorlás.
-   Szombat: 1--2 óra projekt vagy összefoglalás.
-   Vasárnap: opcionális ismétlés.

A terv legyen rugalmas. Ha egy hét kimarad vagy egy téma több időt
igényel, lehessen később folytatni.

A feladatok teljesítése, a jegyzetek és az időbeosztás maradjon meg
újratöltés után is. Első verzióban a localStorage és a JSON
export/import elegendő.

------------------------------------------------------------------------

## 7. A 12 hónapos program végső célja

A program végére szeretnéd:

1.  Megérteni egy teljes BMS-rendszer architektúráját.
2.  Értelmezni a hálózati topológiákat.
3.  IP-címzési és VLAN-terveket készíteni.
4.  Megérteni a routing és firewall szabályok szerepét.
5.  Átlátni a BACnet, Modbus, OPC UA és PROFINET működését.
6.  Megérteni a szerverinfrastruktúra felépítését.
7.  Felismerni az IT/OT biztonsági kockázatokat.
8.  Részt venni egy teljes BMS-rendszer megtervezésében.
9.  Önállóan elkészíteni egy kisebb BMS-rendszer architektúráját és
    dokumentációját.

A hosszú távú szakmai célod tehát:

**BMS Systems Engineer / BMS Architect, erős IT/OT hálózati és
infrastruktúra-ismeretekkel.**

Nem szeretnéd elhagyni a BMS-t, hanem magasabb tervezési és
rendszerarchitekturális szintre szeretnél eljutni.

------------------------------------------------------------------------

## 8. A beszélgetés legfontosabb következtetése

A jelenlegi munkád jó kiindulópont, mert már most találkozol a
BMS-integráció, az ipari protokollok és a valós kommunikációs hibák
problémáival.

A következő fejlődési lépés nem feltétlenül egy munkahelyváltás, hanem a
látóköröd bővítése:

-   ne csak az adatpontot és az integrációt lásd;
-   értsd meg, honnan érkezik az adat;
-   értsd meg, milyen hálózaton halad;
-   tudd, milyen szerver dolgozza fel;
-   értsd meg a biztonsági szabályokat;
-   és idővel vegyél részt abban is, hogy mindezt hogyan kell
    megtervezni.

A gyakorlati első lépés: a következő munkahelyi projektben kérd el a
hálózati topológiai rajzot, próbáld megérteni, készíts róla saját
jegyzetet, és gyűjtsd össze a kérdéseidet.

**A fő elv: lassan, alaposan, gyakorlati példákon keresztül fejlődni --
úgy, hogy közben a BMS maradjon a szakmai fókuszod.**

------------------------------------------------------------------------

## 9. Felülvizsgálat és döntések (2026. november 21.)

> Ez a szakasz utólag került a dokumentumba: a terv szigorú
> felülvizsgálatát és az abból született döntéseket rögzíti. A fenti
> 1--8. szakasz a beszélgetés eredeti összefoglalója, változatlanul.

### A felülvizsgálat fő megállapításai

-   Az új irány illeszkedik a valós munkához (integráció, protokollok,
    hibakeresés); a hálózati tudás a valódi hiány.
-   Ez nem kis módosítás, hanem kb. 80%-os irányváltás a korábbi
    24 hónapos tervhez képest (a cloud/IoT és a szoftverarchitektúra
    kimarad).
-   A terv „BMS-központú", de az eredeti változatban a BMS-tervezés
    (adatpontlista, funkcióleírás, szabályozás) 0% volt, a protokollok
    pedig a deklarált 20% helyett kb. 33%-ot kaptak.
-   A heti 5--7 óra ugyanannyi, mint a leállt tervben, ezért kellett
    újraindító szakasz és „minimum hét".

### Döntések

1.  A régi cloud/IoT és szoftverarchitektúra-tartalom elengedve; az
    MQTT és a Brick/Haystack kis modulként bekerült.
2.  A régi pillérekből csak az angol maradt, heti opcionális pipaként.
3.  Szerkezet: újraindítás (az 1. hónap első két hete heti 2--3 óra),
    „minimum hét" (60 perc tanulás vagy 1 munkahelyi napló-bejegyzés),
    BMS-tervezési szál, egy referencia-épület végig az éven, rugalmas
    sorrend (kitűzhető aktuális hét).
4.  Szoftveres sáv a gyakorlatokban: a protokoll-hónapok gyakorlata
    egy-egy Python-connector („bms-connectors" gyakorló repo), a labor
    Dockerben fut.
5.  Reálisabb 12 hónapos cél: **BMS/OT integrációs mérnök, aki átlátja
    a hálózatot és a teljes rendszert.** A BMS Architect 5+ éves,
    hosszú távú irány.
6.  Piaci visszacsatolás: havi kérdés 3 friss hirdetésről, egyszeri
    LinkedIn/CV-cím frissítés, döntési pont a 3. hónap végén.
7.  A régi 24 hónapos checklist és a napi/heti/havi planner (a régi
    napirend) érintetlen marad, csak a menüből került ki. Közvetlenül
    megnyithatók: `html/roadmap_checklist_24honap.html`,
    `html/napi_heti_honapi_planner.html`.

### Szakmai javítások a tananyagban

-   A „szimbolikus vs. abszolút címzés" S7/PLC-fogalom, nem PROFINET.
    A 8. hónap ezt külön kezeli (S7: PUT/GET, optimized block access);
    a PROFINET IO csak áttekintő szinten szerepel.
-   BACnet: COV, ReadPropertyMultiple, priority array / relinquish,
    network number, BBMD/BDT, BACnet/SC.
-   Modbus: Unit ID és TCP↔RTU gateway, RS-485 alapok.
-   Szerverek: NTP / időszinkron. OT-biztonság: AIC sorrend, vagyis a
    rendelkezésre állás az első.
-   Áttekintés: KNX, DALI, M-Bus. Havonta valódi, ellenőrizhető
    források.

### Piaci kép (2026. november)

-   A pozíciókat másképp hívják: magyarul pl. *épületautomatizálási
    mérnök*, *BMS projektmérnök*, *IT/OT infrastruktúra és hálózati
    mérnök (BMS)*; angolul *BMS / Building Systems Integration
    Engineer*, *Controls Integration Engineer*, *IIoT / OT Engineer*.
-   Keresési tipp: pozíciónév helyett protokollra keress (BACnet,
    Modbus, OPC UA).
-   A hazai BMS-piac kicsi. Az előny a szoftver és az OT metszete,
    ezért a szoftveres láb életben tartása a biztosítás.

### Hol él most a terv

A javított 48 hetes tananyag és a követés: `html/bms_itot_12honap.html`
(a csr-app menüjében: „BMS & IT/OT -- 12 hónapos program"). A
tananyag a fájlban lévő `program-data` JSON-blokkban szerkeszthető.
