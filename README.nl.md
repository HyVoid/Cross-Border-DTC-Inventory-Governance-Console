[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Grensoverschrijdende DTC-voorraadgovernanceconsole
## Opschonen van vraagsignalen, beheersen van pre-orderverplichtingen en inkoopplanning voor Shopify-gebaseerde merken

![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Browser%20%7C%20Excel-success)
![Tool](https://img.shields.io/badge/Tool-Inventory%20Decision%20Support-orange)

**Zet rommelige Shopify-bestelgegevens in enkele minuten om in inkoopbeslissingen—direct in de browser of in de Excel-werkmap, zonder aanmelding, zonder installatie en zonder terugkerend abonnement.**

**Geen aanmelding. Geen installatie. Gratis in uw browser.**

Probeer de browserversie gratis. Als u de Excel-versie nodig hebt, kunt u die kopen met een geld-terug-garantie van 30 dagen zonder vragen.
>
> 🌐 **Openen in de browser** → [*HTML-liveversie*](https://hyvoid.github.io/Cross-Border-DTC-Inventory-Governance-Console/)
>
> 📥 **Excel-versie downloaden**  
> *(GitHub-release / download van de [Website](https://www.theseusworkshop.com/))*

---

## Wat dit helpt te volgen

In plaats van te kijken naar losgekoppelde rapporten uit Shopify, Inventory Planner en spreadsheets, brengt deze console de operationele signalen samen in één besluitingskader.

Het maakt mogelijk om te zien:

- openstaande pre-orderverplichtingen die niet als beschikbare voorraad mogen worden geteld.
- de werkelijke vraag na wegneming van pre-ordervervorming en verwachte retouren.
- inkoophoeveelheden die de feitelijke voorraadverplichtingen weerspiegelen in plaats van opgeblazen verkopen.
- de voorraadverdeling over het VK, de VS, de EU en Australië op basis van de vraagbijdrage.
- synchronisatiegaten tussen Shopify, Inventory Planner en inkoopadministraties voordat ze planningsfouten worden.
- wekelijkse inkoopprioriteiten die steunen op afgestemde operationele gegevens in plaats van handmatige spreadsheetaanpassingen.

---

## Snelstartworkflow

De werkmap is opgebouwd rond een workflow van **eenmalig configureren, regelmatig vernieuwen** in plaats van constant spreadsheetonderhoud.

### 1. Operationele parameters configureren

Open het werkblad **Config** en definieer operationele regels zoals:

- levertijd
- retourvenster
- marktallocatieverhouding
- pre-order-veiligheidsfactor

Deze waarden veranderen meestal alleen wanneer het bedrijfsbeleid verandert.

---

### 2. Bestaande bedrijfsgegevens importeren

Exporteer uw bestaande operationele gegevens uit Shopify en Inventory Planner.

Plak of vernieuw:

- Shopify Orders
- Shopify Returns
- Current Inventory
- Purchase Status

Er is geen herstructurering of handmatige formule-aanpassing nodig.

---

### 3. Automatisch bijgewerkte beslissingen beoordelen

Ga direct naar de analysewerkbladen.

De werkmap vernieuwt onmiddellijk:

- openstaande pre-orderverplichtingen
- cohortretouanalyse
- gecorrigeerde vraag
- inkoopadviezen
- landenallocatie
- afstemmingsstatus

Er zijn geen handmatige berekeningen nodig.

---

### 4. Wekelijks vernieuwen

Elke planningscyclus vervangt eenvoudig de ruwe invoertabellen.

Alles stroomafwaarts werkt automatisch bij.

Er is geen herbouw van de werkmap, geen kopiëren van formules en geen structureel onderhoud.

**Stel een aantal operationele parameters in. Importeer uw bestaande gegevens. Beoordeel de adviezen. Vernieuw zodra nieuwe bedrijfsgegevens beschikbaar zijn.**

---

## Waarom ik dit heb gebouwd

Veel voorraadplanningsproblemen worden niet veroorzaakt door zwakke prognosealgoritmen.

Ze worden veroorzaakt door zwakke vraagsignalen.

Voor merken die meerdere Shopify-webshops runnen, vooral modebedrijven met zware pre-orders en hoge retourpercentages, bevatten de gerapporteerde verkopen vaak signalen die nooit inkoopvraag mogen worden.

Een pre-order wordt als verkoop vastgelegd voordat de voorraad bestaat.

Een geretourneerd artikel keert pas weken later terug in de voorraad.

Voorraadplanners krijgen vaak historische verkopen zonder dat zij een van beide omstandigheden begrijpen.

Het resultaat is voorspelbaar:

- dezelfde vraag twee keer inkopen,
- de toekomstige voorraadbehoefte overschatten,
- onnodige voorraad opstapelen,
- het werkend vermogen verhogen zonder de omzet te verhogen.

---

Ik heb dit project gebouwd omdat ik herhaaldelijk zag dat analisten uren besteedden aan het opschonen van gegevens voordat ze überhaupt met inkoopbeslissingen konden beginnen.

In plaats van nog een dashboard te maken, wilde ik het redeneerproces zelf in een herbruikbare werkmap verpakken.

Bijvoorbeeld:

**Voor**

Een SKU verkoopt **500 eenheden** tijdens een lancering.

De traditionele planning gaat ervan uit dat de vraag gelijk is aan 500.

Inkoopadviezen worden uit dat cijfer gegenereerd.

---

**Na**

De werkmap ontdekt:

- 120 eenheden zijn nog onvervulde pre-orders.
- De verwachte retouren bedragen 48 eenheden.
- De gecorrigeerde vraag wordt **332 eenheden**.

Het inkoopgesprek verandert onmiddellijk.

In plaats van te bespreken hoe snel 500 eenheden worden nabesteld, bespreken operationele teams of 332 eenheden voldoende zijn nadat levertijd en veiligheidsvoorraad zijn meegenomen.

Dat is een wezenlijk andere beslissing—niet omdat de formules veranderden, maar omdat het vraagsignaal betrouwbaar werd.

---

## Veelvoorkomende voorraadplanningsproblemen die dit oplost

| Probleem | Zonder deze tool | Met deze tool |
|----------|-------------------|----------------|
| Pre-orders blazen de vraag op | Inkopen verdubbelen reeds gebonden voorraad | Openstaande verplichtingen worden vóór de prognose geïsoleerd |
| Retouren vervormen historische verkopen | Prognoses gaan ervan uit dat alle verkopen permanente vraag worden | Cohortretourmodellering schat de terug te winnen voorraad |
| Meerdere landen concurreren om voorraad | Handmatige verdeling creëert inconsistente voorraadniveaus | De verdeling volgt configureerbare marktbijdrageverhoudingen |
| Inkoopbeslissingen steunen op niet-verbonden systemen | Analisten vergelijken Shopify, Inventory Planner en ERP handmatig | Geautomatiseerde afstemming markeert afwijkende hoeveelheden |
| Wekelijkse planning vereist herbouw van spreadsheets | Formules kopiëren introduceert verborgen fouten | Ruwe gegevens worden vernieuwd terwijl de berekeningen ongewijzigd blijven |
| Voorraadproblemen worden te laat ontdekt | Inkoopfouten verschijnen na het aanmaken van de inkooporder | Afstemming legt afwijkingen bloot voordat orders worden uitgegeven |

---

## Voor wie dit is

Dit project is ontworpen voor organisaties die voorraadbeslissingen over meerdere markten beheren, waar vraagsignalen worden beïnvloed door pre-orders, retouren en internationale uitvoering.

Typische gebruikers zijn:

- DTC-modemerken
- Shopify-operationele teams
- voorraadplanners
- supply chain-analisten
- assortimentsplanningsteams
- ecommerce-operatiemanagers

Het is bijzonder waardevol waar inkoopbeslissingen afhangen van het begrijpen van het verschil tussen **gerapporteerde verkopen** en **werkelijke voorraadvraag**.

Het is **niet** bedoeld om ERP-platformen, warehouse management-systemen of voorraadsoftware voor bedrijven te vervangen.

In plaats daarvan biedt het een lichtgewicht analytische laag tussen operationele systemen en inkoopbeslissingen.

Er is geen spreadsheet-expertise nodig. Open de browserversie of de Excel-werkmap, importeer uw operationele gegevens en begin direct met het beoordelen van inkoopadviezen.

---

## Over

Ik bouw lichtgewicht analytische werk mappen voor bedrijfssituaties waarin er simpelweg te veel bewegende delen zijn om ze mentaal te doorzien.

In plaats van bedrijfssoftware te vervangen, organiseren deze tools de informatie die nodig is om de volgende operationele beslissing met vertrouwen te nemen.

De **Grensoverschrijdende DTC-voorraadgovernanceconsole** is één voorbeeld van deze aanpak: het omzetten van gefragmenteerde operationele gegevens in een reproduceerbaar besluitingsondersteunend kader dat kan worden vernieuwd zodra nieuwe informatie beschikbaar komt.

## Technische details

<details>
<summary><strong>Voor technische reviewers, Excel-praktijkmensen en medewerkers</strong></summary>

---

## Opbouw van de werkmap

De werkmap volgt een strikte architectuur van **invoer → opschoning → beslissing → validatie → uitvoer**. Elk werkblad heeft één verantwoordelijkheid, wat het analytische proces transparant en controleerbaar maakt.

| Laag | Werkblad | Doel | Afnemer van uitvoer |
|--------|-----------|---------|-----------------|
| Configuratie | Config | Bedrijfsregels, levertijd, allocatieverhoudingen, retourvenster | Alle rekentabellen |
| Ruwe invoer | Raw_Orders | Shopify-bestellexports | Vraagmodule |
| Ruwe invoer | Raw_Returns | Shopify-retourexports | Retourmodel |
| Opschoning | Preorder_Liability | Openstaande pre-orderverplichtingen | Gecorrigeerde vraag, inkoopplanner |
| Opschoning | Cohort_Return_Model | Op cohorts gebaseerd retourgedrag | Gecorrigeerde vraag |
| Beslissing | Corrected_Demand | Ware inkoopvraag | Inventory Planner |
| Beslissing | PO_Planner | Inkoopadviezen | Inkoopteam |
| Beslissing | Location_Allocator | Landenallocatie | Magazijn & logistiek |
| Validatie | Reconciliation | Systeemoverstijgende verificatie | Operaties |
| Presentatie | Executive_Dashboard | Management-KPI's | Directie |

### Algehele gegevensstroom

```text
Shopify Orders
                     \
                      \
                       --> Raw_Orders ------------------\
                                                        \
                                                         \
Inventory Planner Export --> Current Inventory -----------> PO Planner
                                                          /
                                                         /
Shopify Returns --> Raw_Returns --> Cohort Return Model-/

                     Config Parameters
                             │
                             ▼
                 Preorder Liability Engine
                             │
                             ▼
                 Corrected Demand Engine
                             │
                             ▼
                Purchase Recommendation
                             │
                             ▼
                  Country Allocation
                             │
                             ▼
                    Reconciliation
                             │
                             ▼
                 Executive Dashboard
```

Anders dan bij traditionele spreadsheets, waar berekeningen over meerdere werkbladen verspreid zijn, scheidt deze werkmap de operationele verantwoordelijkheden in onafhankelijke analytische lagen.

Die scheiding maakt het mogelijk om elk inkoopadvies terug te voeren naar de operationele gegevens waar het uit voortkomt.

---

## Drie analytische valkuilen die zelfs ervaren voorraadplanners te pakken nemen

---

## Valkuil 1 — Pre-orders behandelen als afgeronde vraag

### Beslissing

Het inkoopteam verhoogt de productie na het waarnemen van ongewoon sterke verkopen.

### Verborgen aanname

Er wordt aangenomen dat de gerapporteerde verkopen de vervulde klantvraag vertegenwoordigen.

In werkelijkheid is een groot deel van die verkopen nog openstaande pre-orders.

### Waarom dit het advies verandert

| Maatstaf | Traditionele zienswijze | Gecorrigeerde zienswijze |
|---------|-----------------|----------------|
| Verkopen | 1.000 | 1.000 |
| Openstaande pre-orders | genegeerd | 280 |
| Inkoopvraag | 1.000 | 720 |

Zonder de openstaande verplichtingen te scheiden, kopen voorraadplanners producten in die klanten al hebben gekocht.

Dat creëert dubbel inkopen.

### Waarom deze redenering verkeerd is

Verkopen beschrijven commerciële activiteit.

Inkopen zou moeten reageren op fysieke voorraadverplichtingen.

Dat is niet altijd hetzelfde.

Vooral bij modelanceringen, crowdfunding en lange productielevertermijnen.

### Gecorrigeerde aanpak

Openstaande pre-orders worden geïsoleerd voordat de vraag het inkoopmodel binnenkomt.

Alleen vervulde vraag draagt bij aan toekomstige inkoopbehoeften.

### Beslissingsresultaat

In plaats van de productie met 1.000 eenheden te verhogen,

kopen operationele teams voorraad voor ongeveer 720 eenheden,

waardoor de onnodige voorraadinvestering daalt terwijl de klantverplichtingen beschermd blijven.

<details>
<summary>Formulelogica</summary>

```excel
Outstanding Liability

=
Total Preorder Sold
-
Fulfilled Preorders
```

Geïmplementeerd met dynamische arrayformules en SUMIFS.

</details>

---

## Valkuil 2 — Retouren meten per kalendermaand

### Beslissing

De directie concludeert dat de retourpercentages zijn gedaald omdat de retouren van deze maand lager lijken.

### Verborgen aanname

Er wordt aangenomen dat retouren die tijdens een kalendermaand plaatsvinden, horen bij verkopen die in diezelfde maand zijn gedaan.

Die aanname is bijna nooit waar.

Retouren zijn gebonden aan inkoopcohorten, niet aan rapportageperioden.

### Waarom dit het advies verandert

Voorbeeld:

| Maand | Verkopen | Kalenderretouren |
|--------|-------|-----------------|
| Januari | 8.000 | 220 |
| Februari | 6.500 | 640 |

Traditionele rapportering suggereert dat februari-producten slechter presteren.

De meeste februari-retouren horen echter in werkelijkbij januari-aankopen.

### Waarom deze redenering verkeerd is

Het klantgedrag volgt de bestelderijd.

Rapporten volgen kalenderdata.

Die tijdlijnen komen zelden overeen.

### Gecorrigeerde aanpak

Bestellingen worden per inkoopcohort gegroepeerd.

Retouren worden gemeten:

- binnen 14 dagen
- binnen 30 dagen
- binnen 45 dagen

Het resulterende retourprofiel weerspiegelt het feitelijke klantgedrag in plaats van rapportage-artefacten.

### Beslissingsresultaat

In plaats van februari-inkopen te verminderen,

ontdekt het bedrijf dat januari-producten vertraagde retouren hebben gekend,

terwijl de februarivraag gezond blijft.

<details>
<summary>Formulelogica</summary>

```excel
Unique Cohort Months

=SORT(
UNIQUE(
TEXT(Order_Date,"yyyy-mm")
))
```

Gecombineerd met MAP(), LET() en SUMIFS() om retourvensters dynamisch te berekenen.

</details>

---

## Valkuil 3 — Inkopen op basis van ruwe verkopen in plaats van gecorrigeerde vraag

### Beslissing

Inventory Planner ontvangt geëxporteerde historische verkopen.

De prognoses lijken redelijk.

Toch creëert inkopen overtollige voorraad.

### Verborgen aanname

Er wordt aangenomen dat historische verkopen al schone vraag vertegenwoordigen.

Dat doen ze zelden.

Historische verkopen bevatten vaak:

- openstaande pre-orders
- verwachte retouren
- tijdelijke lanceringpieken

### Voor

```text
Historical Sales

980
```

Inventory Planner prognosticeert op basis van 980.

### Na opschoning

```text
Historical Sales          980

Outstanding Liability    -170

Expected Returns          -62

Corrected Demand          748
```

### Waarom deze redenering verkeerd is

Prognosealgoritmen versterken de kwaliteit van de invoer.

Ze kunnen zwakke historische signalen niet repareren.

Rommel in levert nog steeds zelfverzekerd uitziende rommel op.

### Gecorrigeerde aanpak

Vraag wordt gecorrigeerd voordat die prognosesoftware binnenkomt.

Inventory Planner ontvangt inkoopvraag in plaats van commerciële activiteit.

### Beslissingsresultaat

Inkoopadviezen worden aanzienlijk stabieler.

Het werkend vermogen daalt terwijl het serviceniveau voor klanten behouden blijft.

<details>
<summary>Formulelogica</summary>

```excel
Corrected Demand

=
Raw Sales
-
Outstanding Liability
-
Expected Returns
```

Geïmplementeerd met LET(), XLOOKUP(), SUMIFS() en dynamische arrays.

</details>

---

## Voorbeeldscenario

Een in het VK gevestigd modemerk brengt een nieuwe jas uit via vier Shopify-webshops die het VK, de VS, de EU en Australië bedienen.

Binnen twee weken meldt Shopify **2.450 verkochte eenheden**, wat op een uiterst succesvolle lancering wijst. Op basis van alleen de ruwe verkopen overweegt het inkoopteam een urgente bijbestelling te plaatsen.

De werkmap vertelt een ander verhaal.

Ten eerste identificeert het werkblad **Preorder_Liability** **540 eenheden** die verkocht maar nog niet vervuld zijn. Deze vertegenwoordigen bestaande klantverplichtingen, geen aanvullende marktvraag.

Vervolgens beoordeelt het **Cohort_Return_Model** het historische retourgedrag voor vergelijkbare producten. Eerdere lanceringen laten een ultiem retourpercentage van **11,8 %** zien, wat erop wijst dat ongeveer **289 eenheden** na levering naar de voorraad terugkeren.

De **Corrected_Demand**-module herrekent vervolgens het inkoopsignaal:

| Post | Hoeveelheid |
|------|---------:|
| Gerapporteerde verkopen | 2.450 |
| Openstaande pre-orders | -540 |
| Verwachte retouren | -289 |
| Gecorrigeerde vraag | **1.621** |

In plaats van tegen het kopcijfer van de verkopen in te kopen, gebruikt **PO_Planner** de gecorrigeerde vraag samen met levertijd, huidige voorraad en veiligheidsparameters om een aanzienlijk kleinere bijbestelhoeveelheid aan te bevelen.

Het advies wordt automatisch verdeeld over de magazijnen in het VK, de VS, de EU en Australië volgens de geconfigureerde allocatieverhoudingen.

Tot slot vergelijkt het werkblad **Reconciliation** de Shopify-verplichtingen met de synchronisatiegegevens van Inventory Planner. Als de openstaande verplichtingen tussen de systemen verschillen, geeft de werkmap een **INVESTIGATE**-waarschuwing voordat inkooporders worden uitgegeven.

Het resultaat is een inkoopbeslissing die steunt op afgestemd operationeel bewijs in plaats van ruwe verkooptotalen, wat overtollige voorraad vermindert terwijl de uitvoeringsverplichtingen aan klanten worden nagekomen.

---

### Formuleverwijzing

<details>
<summary>Config</summary>

| Formule / logica | Doel | Opmerkingen |
|-----------------|---------|------|
| Handmatige configuratie | Definieert operationele parameters | Alleen bijgewerkt wanneer bedrijfsregels veranderen |
| Marktallocatieverhouding | Voorraadverdeling per land | Gebruikt door Location_Allocator |
| Levertijd | Inkoopplanning | Opgenomen in de berekening van de doelvoorraad |
| Retourvenster | Cohortanalyse | Bepaalt de timing van verwachte retouren |
| Pre-order-veiligheidsfactor | Inkoopbuffer | Per markt aanpasbaar |

</details>

---

<details>
<summary>Preorder_Liability</summary>

### Unieke SKU-lijst genereren

```excel
=SORT(
UNIQUE(
Raw_Orders[SKU]
))
```

**Doel**

Maakt een dynamische SKU-hoofdlijst direct uit de geïmporteerde bestelhistorie.

---

### Openstaande pre-orderverplichtingen

```excel
=LET(

SKU_List,A2#,

Preorder_Sold,

SUMIFS(
Raw_Orders[Quantity],
Raw_Orders[SKU],SKU_List,
Raw_Orders[Sales_Type],"Preorder"
),

Preorder_Fulfilled,

SUMIFS(
Raw_Orders[Quantity],
Raw_Orders[SKU],SKU_List,
Raw_Orders[Sales_Type],"Preorder",
Raw_Orders[Fulfillment_Status],"Fulfilled"
),

Preorder_Sold-
Preorder_Fulfilled

)
```

**Doel**

Berekent voorraadverplichtingen die al verkocht maar nog niet fysiek geleverd zijn.

Deze hoeveelheden worden opzettelijk uitgesloten van toekomstige inkoopvraag.

---

</details>

---

<details>
<summary>Cohort_Return_Model</summary>

### Cohortmaanden genereren

```excel
=SORT(
UNIQUE(
TEXT(
Raw_Orders[Order_Date],
"yyyy-mm"
)
))
```

---

### Retourberekening per cohort

Geïmplementeerd met

- LET()
- MAP()
- SUMIFS()

De berekening meet retouren ten opzichte van de oorspronkelijke besteldatum in plaats van kalenderrapportageperioden.

Retourvensters omvatten:

- 14 dagen
- 30 dagen
- 45 dagen

Dit produceert een stabiele schatting van het ultieme retourgedrag.

---

### Ultiem retourpercentage

```text
Ultimate Return Rate

=

Total Returned Quantity

/

Original Cohort Sales
```

De werkmap gebruikt cohortgedrag in plaats van maandelijkse retourpercentages, omdat inkoopbeslissingen afhangen van klantgedrag en niet van rapportageperioden.

</details>

---

<details>
<summary>Corrected_Demand</summary>

### Gecorrigeerd vraagsignaal

```excel
=LET(

RawSales,

SUMIFS(...),

Outstanding,

XLOOKUP(...),

ExpectedReturns,

RawSales*
AverageReturnRate,

ROUND(

RawSales
-
Outstanding
-
ExpectedReturns,

0)

)
```

### Doel

Zet commerciële activiteit om in inkoopvraag.

In plaats van direct uit historische verkopen te voorspellen, verwijdert de werkmap:

- openstaande pre-orders
- voorraad die via klantretouren terug wordt verwacht

Het resulterende signaal is geschikt voor Inventory Planner of vergelijkbare prognosesoftware.

</details>

---

<details>
<summary>PO_Planner</summary>

### Netto-inkoopbehoefte

```text
Net Requirement

=

Target Inventory

-

Current Stock

+

Outstanding Liability
```

---

### Aanbevolen inkoophoeveelheid

```excel
=IF(

NetRequired<=0,

0,

MROUND(

NetRequired,

MOQ

)

)
```

### Doel

Bevilt automatisch inkoophoeveelheden voor en respecteert daarbij de minimumorderhoeveelheden van leveranciers.

In plaats van handmatig afronden te vereisen, zijn inkoopadviezen direct geschikt om inkooporders mee te plaatsen.

</details>

---

<details>
<summary>Location_Allocator</summary>

### Landenallocatie

```excel
=ROUND(

Total_PO

*

Allocation_Ratio,

0
)
```

Elk bestemmingsmagazijn ontvangt voorraad volgens configureerbare marktbijdrageverhoudingen.

Het allocatiemodel kan eenvoudig worden uitgebreid naar extra landen zonder de stroomafwaartse berekeningen te wijzigen.

</details>

---

<details>
<summary>Reconciliation</summary>

### Synchronisatiecontrole

```excel
=IF(

Gap=0,

"PASS",

"INVESTIGATE"

)
```

waarbij

```text
Gap

=

Shopify Unfulfilled

-

Inventory Planner Liability
```

Doel:

Markeert onmiddellijk synchronisatieproblemen voordat inkoopbeslissingen op inconsistente gegevens steunen.

</details>

---

## Validatieregels

| Veld | Validatieregel | Foutgedrag |
|------|-----------------|----------------|
| Market | Moet bestaan in de Config-tabel | Opzoeken levert standaardallocatie of validatiewaarschuwing |
| SKU | Mag niet leeg zijn | Rij wordt uit berekeningen uitgesloten |
| Order_ID | Moet uniek zijn | Waarschuwing dubbele transactie |
| Return_ID | Moet uniek zijn | Waarschuwing dubbele retour |
| Order Date | Geldige datum vereist | Record genegeerd tot correctie |
| Return Date | Mag niet voor Order Date vallen | Validatievlag wordt gegenereerd |
| Quantity | Moet groter zijn dan nul | Rij wordt uitgesloten |
| Return Quantity | Mag de oorspronkelijke hoeveelheid niet overschrijden | Validatiewaarschuwing |
| Sales Type | Alleen Normal of Preorder | Ongeldige categorie wordt gemarkeerd |
| Fulfillment Status | Fulfilled / Unfulfilled | Ongeldige waarden worden uitgesloten |
| Allocation Ratio | Totaal moet gelijk zijn aan 100% | Waarschuwing landenallocatie |
| Lead Time | Niet-negatief geheel getal | Inkoopberekening wordt gestaakt |
| Return Window | Positief geheel getal | Waarschuwing cohortberekening |
| MOQ | Groter dan nul | Inkoopadvies wordt uitgeschakeld |
| Current Inventory | Mag niet negatief zijn | Voorraadwaarschuwing |
| Outstanding Liability | Mag pre-orderverkopen niet overschrijden | Afstemmingsalarm |
| Recommended Purchase Quantity | Afgerond op MOQ | Wordt automatisch aangepast |
| Synchronization Gap | Moet gelijk zijn aan nul | INVESTIGATE-status wordt weergegeven |

</details>

---

## Andere tools in deze serie

Deze werk mappen volgen dezelfde ontwerpfilosofie: lichtgewicht besluitingsondersteunende systemen gebouwd voor terugkerende operationele problemen in plaats van vervanging van bedrijfssoftware.

- **Voorraadvoorspelling & nabestelplanning** — Vraagvoorspelling, berekening van het nabestelpunt en voorraadrisicoanalyse.
- **Construction Estimating System** — Begroting van assemblages, kostenbibliotheken, offertevoorbereiding en projectbudgettering.
- **Marketing Budget Allocation Simulator** — Scenarioplanning voor multichannel-marketinginvesteringen.
- **Multi-Currency Trade Finance Dashboard** — Grensoverschrijdende financiële rapportage en rentabiliteitsanalyse.
- **Coffee Shop Operations Audit Toolkit** — Beoordeling van winkelprestaties en analyse van operationele compliance.
- **Project Management & Progress Billing Console** — Mijlpaalopvolging, facturering en budgetcontrole.

Verdere analytische werk mappen worden gepubliceerd via de GitHub-repository en onze [Website](https://www.theseusworkshop.com/).

---

## Licentie

Dit project is gelicentieerd onder de **Apache License 2.0**.

U mag:

- de werkmap gebruiken voor persoonlijke of commerciële doeleinden.
- het analytische kader aanpassen aan operationele vereisten.
- gewijzigde versies distribueren in overeenstemming met de Apache License 2.0.

Zie het bestand **LICENSE** voor de volledige licentietekst.

---

## Slotopmerkingen

Deze werkmap is bewust gepositioneerd als een **besluitingsondersteunende laag**, niet als vervanging voor ERP-, WMS- of planningsplatformen voor bedrijven.

Het doel is eenvoudig:

- operationele gegevens uit bestaande systemen vastleggen,
- analytische vervormingen vóór de planning wegnemen,
- inkoopadviezen genereren die de werkelijke voorraadverplichtingen weerspiegelen,
- transparante berekeningen leveren die geïnspecteerd, gereproduceerd en gecontroleerd kunnen worden.

In plaats van nog een dashboard toe te voegen, productiseert de werkmap een reproduceerbare voorraadplanningmethodiek die in enkele minuten kan worden vernieuwd en die zowel door operationele gebruikers als technische reviewers wordt begrepen.
