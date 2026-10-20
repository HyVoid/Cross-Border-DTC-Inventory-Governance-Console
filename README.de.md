[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Grenzübergreifende DTC-Inventar-Governance-Konsole
## Bereinigung von Bedarfssignalen, Steuerung von Vorbestellungsverbindlichkeiten und Einkaufsplanung für Shopify-basierte Marken

![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Browser%20%7C%20Excel-success)
![Tool](https://img.shields.io/badge/Tool-Inventory%20Decision%20Support-orange)

**Verwandeln Sie verrauschte Shopify-Bestelldaten in Minuten in Einkaufsentscheidungen—direkt im Browser oder in der Excel-Arbeitsmappe, ohne Registrierung, ohne Installation und ohne wiederkehrendes Abonnement.**

**Keine Registrierung. Keine Installation. Kostenlos in Ihrem Browser.**

Testen Sie die Browser-Version kostenlos. Falls Sie die Excel-Version benötigen, können Sie diese mit einer 30-tägigen Geld-zurück-Garantie ohne Rückfragen erwerben.
>
> 🌐 **Im Browser öffnen** → [*HTML-Live-Version*](https://hyvoid.github.io/Cross-Border-DTC-Inventory-Governance-Console/)
>
> 📥 **Excel-Version herunterladen**  
> *(GitHub-Release / [Website](https://www.theseusworkshop.com/)-Download)*

---

## Was Ihnen bei der Verfolgung hilft

Anstatt getrennte Berichte aus Shopify, Inventory Planner und Tabellenkalkulationen zu betrachten, bündelt diese Konsole die operativen Signale in einem Entscheidungsrahmen.

Sie ermöglicht es Ihnen, Folgendes zu erkennen:

- Offene Vorbestellungsverbindlichkeiten, die nicht als verfügbarer Bestand gezählt werden dürfen.
- Den echten Bedarf nach Entfernung der Vorbestellungsverzerrung und der erwarteten Retouren.
- Einkaufsmengen, die die tatsächlichen Bestandsverpflichtungen abbilden statt aufgeblähte Verkäufe.
- Die Bestandsverteilung auf Großbritannien, die USA, die EU und Australien auf Basis des Bedarfsbeitrags.
- Synchronisationslücken zwischen Shopify, Inventory Planner und Einkaufsunterlagen, bevor sie zu Planungsfehlern werden.
- Wöchentliche Einkaufsprioritäten, die auf abgeglichenen operativen Daten beruhen statt auf manuellen Tabellenanpassungen.

---

## Schnellstart-Ablauf

Die Arbeitsmappe ist um einen Ablauf nach dem Motto **einmal konfigurieren, regelmäßig aktualisieren** aufgebaut statt um ständige Tabellenpflege.

### 1. Betriebsparameter konfigurieren

Öffnen Sie das Arbeitsblatt **Config** und legen Sie betriebliche Regeln fest, etwa:

- Vorlaufzeit
- Retourenfenster
- Marktverteilungsquote
- Vorbestellungs-Sicherheitsfaktor

Diese Werte ändern sich in der Regel nur, wenn sich die Geschäftsrichtlinien ändern.

---

### 2. Vorhandene Geschäftsdaten importieren

Exportieren Sie Ihre vorhandenen operativen Daten aus Shopify und Inventory Planner.

Fügen Sie ein oder aktualisieren Sie:

- Shopify Orders
- Shopify Returns
- Current Inventory
- Purchase Status

Es ist keine Umstrukturierung und keine manuelle Formelanpassung erforderlich.

---

### 3. Automatisch aktualisierte Entscheidungen prüfen

Wechseln Sie direkt zu den Analyse-Arbeitsblättern.

Die Arbeitsmappe aktualisiert sofort:

- Offene Vorbestellungsverbindlichkeiten
- Kohorten-Retourenanalyse
- Bereinigten Bedarf
- Einkaufsempfehlungen
- Länderverteilung
- Abgleichstatus

Es sind keine manuellen Berechnungen erforderlich.

---

### 4. Wöchentlich aktualisieren

Jeder Planungszyklus ersetzt einfach die Roh-Eingabetabellen.

Alles Nachgelagerte aktualisiert sich automatisch.

Es gibt kein Neuaufbauen der Arbeitsmappe, kein Kopieren von Formeln und keine strukturelle Pflege.

**Legen Sie einige Betriebsparameter fest. Importieren Sie Ihre vorhandenen Daten. Prüfen Sie die Empfehlungen. Aktualisieren Sie, wann immer neue Geschäftsdaten vorliegen.**

---

## Warum ich dies entwickelt habe

Viele Probleme der Bestandsplanung werden nicht durch schwache Prognosealgorithmen verursacht.

Sie werden durch schwache Bedarfssignale verursacht.

Bei Marken, die mehrere Shopify-Shops betreiben—insbesondere Modeunternehmen mit starken Vorbestellungen und hohen Retourenquoten—enthalten die ausgewiesenen Verkäufe häufig Signale, die niemals zu Einkaufsbedarf werden dürfen.

Eine Vorbestellung wird als Verkauf erfasst, bevor Bestand existiert.

Ein retournierter Artikel kehrt möglicherweise erst Wochen später in den Bestand zurück.

Bestandsplaner erhalten häufig historische Verkäufe, ohne dass sie einen dieser beiden Umstände verstehen.

Das Ergebnis ist vorhersehbar:

- den gleichen Bedarf doppelt einzukaufen,
- den künftigen Bestandsbedarf zu überschätzen,
- unnötigen Bestand anzuhäufen,
- das Betriebskapital zu erhöhen, ohne die Einnahmen zu erhöhen.

---

Ich habe dieses Projekt entwickelt, weil ich wiederholt beobachtet habe, dass Analysten Stunden mit der Datenbereinigung verbringen, bevor sie überhaupt mit Einkaufsentscheidungen beginnen können.

Anstatt eine weitere Dashboard zu schaffen, wollte ich den Begründungsprozess selbst in eine wiederverwendbare Arbeitsmappe verpacken.

Zum Beispiel:

**Vorher**

Ein Artikel verkauft sich während eines Launchs **500 Einheiten**.

Die traditionelle Planung nimmt an, dass der Bedarf 500 beträgt.

Einkaufsempfehlungen werden aus dieser Zahl erzeugt.

---

**Nachher**

Die Arbeitsmappe erkennt:

- 120 Einheiten sind weiterhin unerfüllte Vorbestellungen.
- Die erwarteten Retouren betragen 48 Einheiten.
- Der bereinigte Bedarf wird **332 Einheiten**.

Das Einkaufsgespräch ändert sich sofort.

Anstatt zu diskutieren, wie schnell 500 Einheiten nachbestellt werden, diskutieren die Betriebsteams, ob 332 Einheiten ausreichen, nachdem Vorlaufzeit und Sicherheitsbestand berücksichtigt sind.

Das ist eine grundlegend andere Entscheidung—nicht weil sich die Formeln geändert haben, sondern weil das Bedarfssignal vertrauenswürdig geworden ist.

---

## Häufige Probleme der Bestandsplanung, die dies löst

| Problem | Ohne dieses Werkzeug | Mit diesem Werkzeug |
|----------|-------------------|----------------|
| Vorbestellungen blähen den Bedarf auf | Einkäufe verdoppeln bereits gebundenen Bestand | Offene Verbindlichkeiten werden vor der Prognose isoliert |
| Retouren verzerren historische Verkäufe | Prognosen nehmen an, dass alle Verkäufe dauerhafte Nachfrage werden | Kohorten-Retourenmodellierung schätzt den rückgewinnbaren Bestand |
| Mehrere Länder konkurrieren um Bestand | Manuelle Verteilung erzeugt inkonsistente Bestandsniveaus | Die Verteilung folgt konfigurierbaren Marktbeitragsquoten |
| Einkaufsentscheidungen stützen sich auf unverbundene Systeme | Analysten vergleichen Shopify, Inventory Planner und ERP manuell | Der automatisierte Abgleich hebt abweichende Mengen hervor |
| Wöchentliche Planung erfordert Neuaufbau von Tabellen | Formelkopieren führt versteckte Fehler ein | Rohdaten werden aktualisiert, während die Berechnungen unverändert bleiben |
| Bestandsprobleme werden zu spät entdeckt | Einkaufsfehler erscheinen nach der Erstellung der Bestellung | Der Abgleich deckt Abweichungen vor der Auftragserteilung auf |

---

## Für wen dies gedacht ist

Dieses Projekt ist für Organisationen gedacht, die Bestandsentscheidungen über mehrere Märkte hinweg steuern, wo Bedarfssignale durch Vorbestellungen, Retouren und internationale Erfüllung beeinflusst werden.

Typische Nutzer sind:

- DTC-Modemarken
- Shopify-Betriebsteams
- Bestandsplaner
- Lieferkettenanalysten
- Warenplanungsteams
- Ecommerce-Betriebsleiter

Es ist besonders wertvoll, wo Einkaufsentscheidungen davon abhängen, den Unterschied zwischen **ausgewiesenen Verkäufen** und **echtem Bestandsbedarf** zu verstehen.

Es ist **nicht** dazu bestimmt, ERP-Plattformen, Lagerverwaltungssysteme oder Bestandssoftware für Unternehmen zu ersetzen.

Stattdessen bietet es eine leichtgewichtige analytische Schicht zwischen operativen Systemen und Einkaufsentscheidungen.

Es ist keine Tabellenkalkulations-Expertise erforderlich. Öffnen Sie die Browser-Version oder die Excel-Arbeitsmappe, importieren Sie Ihre operativen Daten und beginnen Sie sofort mit der Prüfung der Einkaufsempfehlungen.

---

## Über

Ich entwickle leichtgewichtige analytische Arbeitsmappen für Geschäftssituationen, in denen es schlicht zu viele bewegliche Teile gibt, um sie im Kopf zu durchdenken.

Anstatt Unternehmenssoftware zu ersetzen, organisieren diese Werkzeuge die Informationen, die benötigt werden, um die nächste betriebliche Entscheidung mit Zuversicht zu treffen.

Die **Grenzübergreifende DTC-Inventar-Governance-Konsole** ist ein Beispiel für diesen Ansatz: die Umwandlung fragmentierter operativer Daten in einen wiederholbaren Entscheidungsunterstützungsrahmen, der aktualisiert werden kann, wann immer neue Informationen vorliegen.

## Technische Details

<details>
<summary><strong>Für technische Prüfer, Excel-Praktiker und Mitwirkende</strong></summary>

---

## Aufbau der Arbeitsmappe

Die Arbeitsmappe folgt einer strengen Architektur aus **Eingabe → Bereinigung → Entscheidung → Validierung → Ausgabe**. Jedes Arbeitsblatt hat eine einzige Verantwortung, wodurch der analytische Prozess transparent und prüfbar wird.

| Schicht | Arbeitsblatt | Zweck | Ausgabeverbraucher |
|--------|-----------|---------|-----------------|
| Konfiguration | Config | Geschäftsregeln, Vorlaufzeit, Verteilungsquoten, Retourenfenster | Alle Berechnungsblätter |
| Rohn-Eingabe | Raw_Orders | Shopify-Bestellexporte | Bedarfsmodul |
| Rohn-Eingabe | Raw_Returns | Shopify-Retourenexporte | Retourenmodell |
| Bereinigung | Preorder_Liability | Offene Vorbestellungsverpflichtungen | Bereinigter Bedarf, Einkaufsplaner |
| Bereinigung | Cohort_Return_Model | Kohortenbasiertes Retourenverhalten | Bereinigter Bedarf |
| Entscheidung | Corrected_Demand | Echter Einkaufsbedarf | Inventory Planner |
| Entscheidung | PO_Planner | Einkaufsempfehlungen | Einkaufsteam |
| Entscheidung | Location_Allocator | Länderverteilung | Lager & Logistik |
| Validierung | Reconciliation | systemübergreifende Verifizierung | Betrieb |
| Darstellung | Executive_Dashboard | Management-Kennzahlen | Geschäftsführung |

### Gesamter Datenfluss

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

Anders als bei traditionellen Tabellenkalkulationen, wo Berechnungen über mehrere Arbeitsblätter verstreut sind, trennt diese Arbeitsmappe die betrieblichen Verantwortlichkeiten in unabhängige analytische Schichten.

Diese Trennung ermöglicht es, jede Einkaufsempfehlung auf ihre ursprünglichen operativen Daten zurückzuverfolgen.

---

## Drei analytische Fallen, die auch erfahrene Bestandsplaner stellen

---

## Falle 1 — Vorbestellungen als abgeschlossene Nachfrage behandeln

### Entscheidung

Das Einkaufsteam erhöht die Produktion, nachdem es ungewöhnlich starke Verkäufe beobachtet.

### Verborgene Annahme

Es wird angenommen, dass die ausgewiesenen Verkäufe den erfüllten Kundendbedarf darstellen.

In Wirklichkeit ist ein großer Teil dieser Verkäufe weiterhin offene Vorbestellungen.

### Warum dies die Empfehlung ändert

| Kennzahl | Traditionelle Sicht | Bereinigte Sicht |
|---------|-----------------|----------------|
| Verkäufe | 1.000 | 1.000 |
| Offene Vorbestellungen | ignoriert | 280 |
| Einkaufsbedarf | 1.000 | 720 |

Ohne die offenen Verbindlichkeiten zu trennen, kaufen Bestandsplaner Produkte ein, die Kunden bereits gekauft haben.

Dies erzeugt doppelten Einkauf.

### Warum diese Begründung falsch ist

Verkäufe beschreiben kommerzielle Aktivität.

Der Einkauf sollte auf physische Bestandsverpflichtungen reagieren.

Das ist nicht immer dasselbe.

Insbesondere bei Modelaunchs, Crowdfunding und langen Fertigungsvorlaufzeiten.

### Korrigierter Ansatz

Offene Vorbestellungen werden isoliert, bevor der Bedarf in das Einkaufsmodell eingeht.

Nur erfüllter Bedarf trägt zu künftigen Einkaufsanforderungen bei.

### Ergebnis der Entscheidung

Anstatt die Produktion um 1.000 Einheiten zu erhöhen,

kaufen die Betriebsteams Bestand für etwa 720 Einheiten,

was die unnötige Bestandsinvestition verringert und gleichzeitig die Kundenverpflichtungen schützt.

<details>
<summary>Formellogik</summary>

```excel
Outstanding Liability

=
Total Preorder Sold
-
Fulfilled Preorders
```

Implementiert mit dynamischen Array-Formeln und SUMIFS.

</details>

---

## Falle 2 — Retouren nach Kalendermonat messen

### Entscheidung

Die Geschäftsführung schließt, dass die Retourenquoten gefallen sind, weil die Retouren dieses Monats niedriger erscheinen.

### Verborgene Annahme

Es wird angenommen, dass Retouren, die in einem Kalendermonat auftreten, zu Verkäufen gehören, die im selben Monat getätigt wurden.

Diese Annahme ist fast nie richtig.

Retouren sind an Einkaufskohorten gebunden, nicht an Berichtszeiträume.

### Warum dies die Empfehlung ändert

Beispiel:

| Monat | Verkäufe | Kalenderretouren |
|--------|-------|-----------------|
| Januar | 8.000 | 220 |
| Februar | 6.500 | 640 |

Die traditionelle Berichterstattung legt nahe, dass Februar-Produkte schlechter abschneiden.

Allerdings gehören die meisten Februar-Retouren tatsächlich zu Januar-Käufen.

### Warum diese Begründung falsch ist

Das Kundenverhalten folgt dem Bestellalter.

Berichte folgen Kalenderdaten.

Diese Zeitlinien stimmen selten überein.

### Korrigierter Ansatz

Bestellungen werden nach Einkaufskohorte gruppiert.

Retouren werden gemessen:

- innerhalb von 14 Tagen
- innerhalb von 30 Tagen
- innerhalb von 45 Tagen

Das resultierende Retourenprofil spiegelt das tatsächliche Kundenverhalten wider statt Berichtungsartefakte.

### Ergebnis der Entscheidung

Anstatt die Februar-Einkäufe zu verringern,

entdeckt das Unternehmen, dass Januar-Produkte verspätete Retouren erlebt haben,

während die Februar-Nachfrage gesund bleibt.

<details>
<summary>Formellogik</summary>

```excel
Unique Cohort Months

=SORT(
UNIQUE(
TEXT(Order_Date,"yyyy-mm")
))
```

Kombiniert mit MAP(), LET() und SUMIFS(), um Retourenfenster dynamisch zu berechnen.

</details>

---

## Falle 3 — Einkauf aus Rohverkäufen statt aus bereinigtem Bedarf

### Entscheidung

Inventory Planner erhält exportierte historische Verkäufe.

Die Prognosen erscheinen angemessen.

Der Einkauf erzeugt dennoch überschüssigen Bestand.

### Verborgene Annahme

Es wird angenommen, dass historische Verkäufe bereits sauberen Bedarf darstellen.

Das tun sie selten.

Historische Verkäufe enthalten häufig:

- offene Vorbestellungen
- erwartete Retouren
- temporäre Launch-Ausschläge

### Vorher

```text
Historical Sales

980
```

Inventory Planner prognostiziert ausgehend von 980.

### Nach der Bereinigung

```text
Historical Sales          980

Outstanding Liability    -170

Expected Returns          -62

Corrected Demand          748
```

### Warum diese Begründung falsch ist

Prognosealgorithmen verstärken die Eingabequalität.

Sie können schwache historische Signale nicht reparieren.

Müll herein produziert weiterhin selbstsicher aussehenden Müll heraus.

### Korrigierter Ansatz

Der Bedarf wird korrigiert, bevor er in Prognosesoftware eingeht.

Inventory Planner erhält Einkaufsbedarf statt kommerzielle Aktivität.

### Ergebnis der Entscheidung

Einkaufsempfehlungen werden deutlich stabiler.

Das Betriebskapital sinkt, während das Kundendienstniveau gehalten wird.

<details>
<summary>Formellogik</summary>

```excel
Corrected Demand

=
Raw Sales
-
Outstanding Liability
-
Expected Returns
```

Implementiert mit LET(), XLOOKUP(), SUMIFS() und dynamischen Arrays.

</details>

---

## Beispielszenario

Eine in Großbritannien ansässige Modemarke bringt eine neue Jacke über vier Shopify-Shops auf den Markt, die Großbritannien, die USA, die EU und Australien bedienen.

Innerhalb von zwei Wochen meldet Shopify **2.450 verkaufte Einheiten**, was auf einen sehr erfolgreichen Launch hindeutet. Allein auf Basis der Rohverkäufe erwägt das Einkaufsteam eine dringende Nachbestellung.

Die Arbeitsmappe erzählt eine andere Geschichte.

Zunächst identifiziert das Arbeitsblatt **Preorder_Liability** **540 Einheiten**, die verkauft, aber noch nicht erfüllt wurden. Diese stellen bestehende Kundenverpflichtungen dar, keine zusätzliche Marktnachfrage.

Anschließend bewertet das **Cohort_Return_Model** das historische Retourenverhalten vergleichbarer Produkte. Frühere Launchs zeigen eine ultimative Retourenquote von **11,8 %**, was darauf hindeutet, dass etwa **289 Einheiten** nach der Lieferung in den Bestand zurückkehren werden.

Das **Corrected_Demand**-Modul berechnet dann das Einkaufssignal neu:

| Posten | Menge |
|------|---------:|
| Ausgewiesene Verkäufe | 2.450 |
| Offene Vorbestellungen | -540 |
| Erwartete Retouren | -289 |
| Bereinigter Bedarf | **1.621** |

Anstatt gegen die Hauptverkaufszahl einzukaufen, verwendet **PO_Planner** den bereinigten Bedarf zusammen mit Vorlaufzeit, aktuellem Bestand und Sicherheitsparametern, um eine deutlich kleinere Nachbestellmenge zu empfehlen.

Die Empfehlung wird automatisch auf die Lager in Großbritannien, den USA, der EU und Australien gemäß den konfigurierten Verteilungsquoten verteilt.

Schließlich vergleicht das Arbeitsblatt **Reconciliation** die Shopify-Verbindlichkeiten mit den Synchronisationsdaten von Inventory Planner. Wenn sich die offenen Verpflichtungen zwischen den Systemen unterscheiden, löst die Arbeitsmappe eine **INVESTIGATE**-Warnung aus, bevor Bestellungen erteilt werden.

Das Ergebnis ist eine Einkaufsentscheidung, die auf abgeglichenen operativen Belegen beruht statt auf Rohverkaufssummen, wodurch überschüssiger Bestand reduziert und gleichzeitig die Kundenerfüllungsverpflichtungen gehalten werden.

---

### Formelreferenz

<details>
<summary>Config</summary>

| Formel / Logik | Zweck | Hinweise |
|-----------------|---------|------|
| Manuelle Konfiguration | Legt Betriebsparameter fest | Wird nur bei Änderung der Geschäftsregeln gepflegt |
| Marktverteilungsquote | Länderbestandsverteilung | Wird von Location_Allocator verwendet |
| Vorlaufzeit | Einkaufsplanung | Geht in die Berechnung des Zielbestands ein |
| Retourenfenster | Kohortenanalyse | Steuert den erwarteten Retourenzeitpunkt |
| Vorbestellungs-Sicherheitsfaktor | Einkaufspuffer | Je Markt anpassbar |

</details>

---

<details>
<summary>Preorder_Liability</summary>

### Eindeutige SKU-Liste erzeugen

```excel
=SORT(
UNIQUE(
Raw_Orders[SKU]
))
```

**Zweck**

Erzeugt eine dynamische SKU-Stammliste direkt aus der importierten Bestellhistorie.

---

### Offene Vorbestellungsverbindlichkeiten

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

**Zweck**

Berechnet Bestandsverpflichtungen, die bereits verkauft, aber physisch noch nicht geliefert wurden.

Diese Mengen werden absichtlich vom künftigen Einkaufsbedarf ausgeschlossen.

---

</details>

---

<details>
<summary>Cohort_Return_Model</summary>

### Kohortenmonate erzeugen

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

### Kohorten-Retourenberechnung

Implementiert mit

- LET()
- MAP()
- SUMIFS()

Die Berechnung misst Retouren relativ zum ursprünglichen Bestelldatum, nicht zu Kalender-Berichtszeiträumen.

Retourenfenster umfassen:

- 14 Tage
- 30 Tage
- 45 Tage

Dies erzeugt eine stabile Schätzung des ultimativen Retourenverhaltens.

---

### Ultimative Retourenquote

```text
Ultimate Return Rate

=

Total Returned Quantity

/

Original Cohort Sales
```

Die Arbeitsmappe verwendet Kohortenverhalten statt monatlicher Retourenquoten, weil Einkaufsentscheidungen vom Kundenverhalten abhängen, nicht von Berichtszeiträumen.

</details>

---

<details>
<summary>Corrected_Demand</summary>

### Bereinigtes Bedarfssignal

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

### Zweck

Verwandelt kommerzielle Aktivität in Einkaufsbedarf.

Anstatt direkt aus historischen Verkäufen zu prognostizieren, entfernt die Arbeitsmappe:

- offene Vorbestellungen
- Bestand, der über Kundenretouren erwartet zurückkehrt

Das resultierende Signal ist für Inventory Planner oder ähnliche Prognosesoftware geeignet.

</details>

---

<details>
<summary>PO_Planner</summary>

### Netto-Einkaufsbedarf

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

### Empfohlene Einkaufsmenge

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

### Zweck

Empfiehlt automatisch Einkaufsmengen und respektiert dabei die Mindestbestellmengen der Lieferanten.

Anstatt manuelles Runden zu erfordern, sind Einkaufsempfehlungen sofort zur Erteilung von Bestellungen geeignet.

</details>

---

<details>
<summary>Location_Allocator</summary>

### Länderverteilung

```excel
=ROUND(

Total_PO

*

Allocation_Ratio,

0
)
```

Jedes Ziellager erhält Bestand gemäß den konfigurierbaren Marktbeitragsquoten.

Das Verteilungmodell kann leicht auf weitere Länder erweitert werden, ohne nachgelagerte Berechnungen zu ändern.

</details>

---

<details>
<summary>Reconciliation</summary>

### Synchronisationsprüfung

```excel
=IF(

Gap=0,

"PASS",

"INVESTIGATE"

)
```

wobei

```text
Gap

=

Shopify Unfulfilled

-

Inventory Planner Liability
```

Zweck:

Hebt sofort Synchronisationsprobleme hervor, bevor Einkaufsentscheidungen auf inkonsistenten Daten beruhen.

</details>

---

## Validierungsregeln

| Feld | Validierungsregel | Fehlerverhalten |
|------|-----------------|----------------|
| Market | Muss in der Config-Tabelle existieren | Nachschlagen liefert Standardverteilung oder Validierungswarnung |
| SKU | Darf nicht leer sein | Zeile wird von Berechnungen ausgeschlossen |
| Order_ID | Muss eindeutig sein | Warnung bei doppelter Transaktion |
| Return_ID | Muss eindeutig sein | Warnung bei doppelter Retoure |
| Order Date | Gültiges Datum erforderlich | Datensatz wird bis zur Korrektur ignoriert |
| Return Date | Darf nicht vor Order Date liegen | Validierungsflag wird erzeugt |
| Quantity | Muss größer als null sein | Zeile wird ausgeschlossen |
| Return Quantity | Darf die ursprüngliche Menge nicht überschreiten | Validierungswarnung |
| Sales Type | Nur Normal oder Preorder | Ungültige Kategorie wird hervorgehoben |
| Fulfillment Status | Fulfilled / Unfulfilled | Ungültige Werte werden ausgeschlossen |
| Allocation Ratio | Summe muss 100 % betragen | Warnung zur Länderverteilung |
| Lead Time | Nicht negative Ganzzahl | Einkaufsberechnung wird angehalten |
| Return Window | Positive Ganzzahl | Warnung zur Kohortenberechnung |
| MOQ | Größer als null | Einkaufsempfehlung wird deaktiviert |
| Current Inventory | Darf nicht negativ sein | Bestandswarnung |
| Outstanding Liability | Darf Vorbestellungsverkäufe nicht überschreiten | Abgleichsalarm |
| Recommended Purchase Quantity | Auf MOQ gerundet | Wird automatisch angepasst |
| Synchronization Gap | Muss null betragen | INVESTIGATE-Status wird angezeigt |

</details>

---

## Weitere Werkzeuge dieser Reihe

Diese Arbeitsmappen folgen derselben Entwurfsphilosophie: leichtgewichtige Entscheidungsunterstützungssysteme für wiederkehrende betriebliche Probleme statt Ersatz für Unternehmenssoftware.

- **Bestandsprognose & Nachbestellungsplanung** — Bedarfsprognose, Bestellpunktberechnung und Bestandsrisikoanalyse.
- **Construction Estimating System** — Kalkulation von Baugruppen, Kostenbibliotheken, Angebotsvorbereitung und Projektbudgetierung.
- **Marketing Budget Allocation Simulator** — Szenarioplanung für mehrkanalige Marketinginvestitionen.
- **Multi-Currency Trade Finance Dashboard** — Grenzüberschreitende Finanzberichterstattung und Rentabilitätsanalyse.
- **Coffee Shop Operations Audit Toolkit** — Filialleistungsprüfung und Analyse der betrieblichen Compliance.
- **Project Management & Progress Billing Console** — Meilensteinverfolgung, Rechnungsstellung und Budgetkontrolle.

Weitere analytische Arbeitsmappen werden über das GitHub-Repository und unsere [Website](https://www.theseusworkshop.com/) veröffentlicht.

---

## Lizenz

Dieses Projekt ist unter der **Apache License 2.0** lizenziert.

Sie dürfen:

- Die Arbeitsmappe für persönliche oder kommerzielle Zwecke verwenden.
- Den analytischen Rahmen an betriebliche Anforderungen anpassen.
- Veränderte Versionen gemäß der Apache License 2.0 verteilen.

Siehe die Datei **LICENSE** für den vollständigen Lizenztext.

---

## Abschließende Hinweise

Diese Arbeitsmappe ist absichtlich als **Entscheidungsunterstützungsschicht** positioniert, nicht als Ersatz für ERP-, WMS- oder Unternehmensplanungsplattformen.

Ihr Zweck ist unkompliziert:

- operative Daten aus bestehenden Systemen zu erfassen,
- analytische Verzerrungen vor der Planung zu entfernen,
- Einkaufsempfehlungen zu erzeugen, die die echten Bestandsverpflichtungen abbilden,
- transparente Berechnungen zu liefern, die geprüft, reproduziert und auditiert werden können.

Anstatt ein weiteres Dashboard hinzuzufügen, produktisiert die Arbeitsmappe eine wiederholbare Bestandsplanungsmethodik, die in Minuten aktualisiert und von betrieblichen Nutzern und technischen Prüfern gleichermaßen verstanden werden kann.
