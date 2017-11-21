---
title: "Vorlesung 6: Anforderungsanalyse"
date: "20/11/2017"
---

## Vorlesung 6: Anforderungsanalyse mit UML-Use Case Diagramm, Satzschablone und textueller Use Case Definition

## Anforderungsanalyse

### Satzschablonen für die Anforderungsermittlung

#### Visualisierung der Systemaktivitäten
<img src="./images/umlUseCase/visualisierungsystemaktivitaeten.png" width="600">

#### Charakterisierung der Systemaktivitäten
1. Selbstständige Systemaktivität
  Das System **führt** den Prozess selbstständig durch.
2. Benutzerinteraktion
  Das System **stellt** dem Nutzer die Prozessfunktionalität zur Verfügung.
3. Schnittstellenanforderung:
  Das System führt einen Prozess in Abhängigkeit von einem Dritten (zum Beispiel einem Fremdsystem) aus, ist an sich passiv und wartet auf ein externes Ereignis.

#### Satzschablone nach Rupp
<img src="./images/umlUseCase/satzschablone.png" width="600">

##### Selbstständige Systemaktivität Beispiele
* Nach der Eingabe eines neuen Teilprojekts und nach der Aktualisierung des Aufwandes eines Teilprojekts oder einer neuen Projektaufgabe muss das System die **Aufwandsangaben auf Plausibilität** prüfen.
* Falls der eingegebene Bibliothekskunde bereits im System vorhanden ist, muss das System die Fehlermeldung "Kunde vorhanden" ausgeben.

##### Benutzer Interaktion Beispiele
* In der Projektbearbeitung muss das System dem Nutzer die Möglichkeit bieten, ein **neues Projekt** mit Projektausgangsdaten anzulegen.
* Nach der Projektauswahl muss das System dem Nutzer die Möglichkeit bieten, für **existierende Projekte** neue Teilprojekte anzulegen.
* Nachdem das System die Geschäftsdaten gespeichert hat, muss das System dem Mitarbeiter die Möglichkeit bieten, einen **Genehmigungsantrag auf dem Netzwerkdrucker zu drucken**.
* Das System muss dem Sachbearbeiter die Möglichkeit bieten, **neue Dozenten zu erfassen**.

##### Schnittstellenanforderung
* Nach der Kontaktaufnahme durch die Software „Globalview“ muss das System fähig sein, Anfragen nach den Projektnamen, deren Gesamtaufwänden und Fertigstellungsgraden anzunehmen.
* Das Personalmodul wird fähig sein, Personendaten aus der Datenbank zu importieren.

#### Verbindlichkeit
| Rechtliche Verbindlichkeit | Schlüsselwort |
|---|:---:|
| Der Ausdruck *muss*, wird benutzt um verpflichtende Anforderungen zu definieren. | **muss** |
| Der Ausdruck *sollte*, wird benutzt um wünschenswerte Anforderungen zu definieren. | **sollte** |
| Der Ausdruck *wird*, wird benutzt, um Anforderungen zu definieren, die in der Zukunft integriert werden. | **wird** |

#### Prozesse
| Prozesswort | Semantische Definition des Prozesswortes | Synonyme |
|:---:|---|---|
| speichern | Im Bibliothekssystem muss *speichern* den Prozess bedeuten, Informationen persistent aufzubewahren. | sammeln, aufbewahren |
| auswählen | Im Bibliothekssystem muss *auswählen* den Prozess bedeuten, eines oder mehrere Elemente aus einer endlichen Menge von Elementen zu bestimmen. | selektieren, markieren |
| anzeigen | Im Bibliothekssystem muss *anzeigen* den Prozess bedeuten, dem Benutzer Informationen auf dem Bildschirm darzustellen. | darstellen, ausgeben |
| einfügen | Im Bibliothekssystem muss *einfügen* den Prozess bedeuten, neue Daten einzugeben oder vorhandene Daten zu überschreiben. | eingeben, einsetzen |

#### Bedingungen
| Bedingung | Logische Bedingung | Zeitliche Bedingung | Semantische Definition der Bedingung |
|:---:|:---:|:---:|---|
| FALLS | X | - | Das Wort *falls* bedeutet, dass das System eine Aufgabe bearbeitet, falls bestimmte Logische Bedingungen wahr sind. |
| NACHDEM | - | X | Das Wort *nachdem* bedeutet, dass ein System eine gestartete Aufgabe erst vollständig abgearbeitet haben muss, bevor das System eine neue Aufgabe beginnt. |
| SOBALD | - | X | Das Wort *sobald* bedeutet, dass ein System eine gestartete Aufgabe **nicht** vollständig abgearbeitet haben muss, bevor das System eine neue Aufgabe beginnt. |
| SOLANGE | - | X | Das Wort *solange* bedeutet, dass das System eine bereits gestartete Aufgabe **nicht** vollständig abgearbeitet haben muss, bevor das System eine weitere Aufgabe beginnt. Die neu gestartete Aufgabe wird exakt solange ausgeführt, wie die vorher bereits gestartete Aufgabe andauert. |

<img src="./images/umlUseCase/if.png" width="600">

### Was ist ein Anwendungsfall(Use Case)?

#### Definition
* Eine Use Case
 * definiert die funktionalen Hauptaufgaben eines Systems
 * beschreibt in der Sprache der Stakeholder eine konsistente und zielgerichtete Interaktion des Benutzers mit einem System
 * beschreibt das gewünschte Systemverhalten aus der Sicht des Anwenders und somit Anforderungen, die das System erfüllen soll
 * beschreibt, was das System leisten muss, aber nicht, wie es dies leisten soll
 * besteht aus mehreren zusammenhängenden Aufgaben, die von einem Akteur durchgeführt werden, um ein Ziel zu erreichen bzw. ein gewünschtes Ergebnis zu erstellen

* Alle Anwendungsfälle zusammen dokumentieren die Möglichkeiten der Benutzung des Softwaresystems und werden in einem Use Case Diagramm dargestellt.

#### Use Case vs. User Story
* Eine User Story ist eine einfache kurze Beschreibung eines Benutzerziels, um einen Nutzen zu generieren
* Ein Use Case ist die detaillierte Spezifikation von Funktionalität (Reihenfolge von Systemaktivitäten), um ein gewünschtes Resultat zu erzielen
* Use Cases fokussieren auf Nutzerinteraktionen mit einem System, so dass das Ziel der Nutzer klar wird
* Use Cases können mit include- und extends-Beziehungen strukturiert werden
* User Stories eignen sich für inkrementelles Vorgehen, während Use Cases sich gut für eine Neuentwicklung eignen
* User Stories werden im Gegensatz zu Use Cases nicht als Instrument zur  Dokumentation eingesetzt, sondern als Basis, um über Anforderungen zu reden
* User Stories werden als Planungsinstrument eingesetzt und so lange kompakt „kleingeschnitten“, bis sie in einem festgelegten Zeitraum einer Iteration umgesetzt werden können

### Szenario

#### Anwendungsfall
Beschreibt eine abstrakte Interaktion zwischen Akteuren und dem System

#### Szenario
Eine konkrete Ausprägung eines Anwendungsfalls. Das bedeutet ein möglicher Ablauf mit konkreten Werten.
Ein Szenario ist eine Instanz eines Anwendungsfalls.

* Szenarien sind Beschreibungen des Systems, wie es in der Praxis benutzt wird
* Ein Anwendungsfall kann mehrere Szenarien haben
* Szenarien sind hilfreich bei der Anforderungsermittlung, da Personen diese besser verstehen als abstrakte Angaben
* Szenarien können durch Interaktionsdiagramme (Sequenzdiagramm, Kommunikationsdiagramm) dargestellt werden
* Ein Szenario beschreibt eine Abfolge von Schritten, die vom Use Case zu durchlaufen sind
    * __Normalabläufe__ zeigen auf, wie der Anwendungsfall "normalerweise" (erfolgreich) abläuft
    * __Alternativabläufe__ zeigen "andere" Wege zum Ziel auf, als dies im Normalablauf dargestellt wird
    * __Ausnahmeabläufe__ führen nicht zum Ziel, z.B. infolge eines "fachlichen Fehlers" oder bei einem Abbruch durch den Akteur

<img src="./images/umlUseCase/szenario.png" width="600">

### Notationselemente für Use Case Diagramme

<img src="./images/umlUseCase/useCaseVerkauf.png" width="600">

* <span style="color:red">Achtung: Kunde nicht gefunden ist kein geeigneter Use Case</span>
* <span style="color:red">UC-Name wie „Kundendaten einsehen“ immer in den Use Case schreiben</span>

#### Was ist ein Akteur(Aktor) ?

* Rolle, die Benutzer eines Systems spielt
* Häufig eine Person
* Kann auch eine Organisationsheit oder ein System sein
* Befindet sich immer außerhalb des Systems

** Notation:** <img src="./images/umlUseCase/Akteure.png" width="300" align="middle">

#### Arten von Aktoren

* Meschlich: Anfänger, geübter Benutzer, Admin
* Nicht-Menschlich: Messaging-System, E-Mail System
* Primär: Hauptnutzer des Systems
* Sekundär: notwendig für das Funktionieren des Systems
* Aktiv: stößt selbst Anwendungsfälle an
* Passiv: stößt keine Anwendungsfälle an

Beispiel: <img src="./images/umlUseCase/artenAktor.png" width="600" align="middle">


#### Notation

<img src="./images/umlUseCase/notation.png" width="600" align="middle">

<img src="./images/umlUseCase/notation2.png" width="600" align="middle">

#### Vererbung bei Akteuren und Kardinalitäten

<img src="./images/umlUseCase/vererbung.png" width="600" align="middle">

#### Use-Case Diagramm: Generalisierung

<img src="./images/umlUseCase/generalisierung.png" width="200">


Use-Case B erbt alle Aktionen und Eigenschaften von Use- Case A. Auch die Beziehungen zu verschiedenen Akteuren werden vererbt.

Use-Case B kann Aktionen von Use-Case-A verfeinern, indem bestimmte Aktionen überschrieben werden

#### Use-Case Diagramm: Include

<img src="./images/umlUseCase/include.png" width="300">


Die «include»-Beziehung visualisiert, dass ein Use-Case (A) das Verhalten eines anderen Use-Case (B) importiert. Die Beziehung ist nicht optional, so dass  das Verhalten immer importiert wird

Erst die Beschreibung der Aktionen definiert, an welcher Stelle der Use-Case B inkludiert wird.

#### Use-Case Diagramm: Extend

<img src="./images/umlUseCase/extend.png" width="300">

Die «extend»-Beziehung zeigt an, dass das Verhalten eines Use-Case (A) durch einen anderen Use-Case (B) erweitert werden kann, aber nicht muss.

Den Zeitpunkt, an dem ein Verhalten eines Use-Case erweitert werden kann, bezeichnet man als Erweiterungspunkt (engl. extension point). Ein Use-Case darf mehrere Erweiterungspunkte besitzen.

Eine Erweiterung kann noch um eine optionale Bedingung ergänzt werden. D.h. nur wenn die Bedigung erfüllt ist, wird die Erweiterung tatsächlich ausgeführt

Beispiele

<img src="./images/umlUseCase/beispielExtendInclude.png" width="500">

<img src="./images/umlUseCase/Einweihungsfeier.png" width="500">

<img src="./images/umlUseCase/Bierzelt.png" width="500">

### Best Practices

* Use Cases sollen eine Sinvolle Bezeichnung, die aus einem Substantiv und aktivem Verb bestehen.
* Die Sprache soll standardisiert sein und Konsistenz haben.
* Keine Abläufe modellieren
* Aktor immer Außerhalb des Systems
* Keine Unterschiedlichen Benutzer mit Zuständen ("Benutzer" & "Registrierter Benutzer")
* Use Cases nicht zu umfangreich
* Auf die wichtigsten **include** und **extends** konzentrieren
* Große Diagramme in mehrere aufteilen
* Use Case mit mehreren Akteuren
   * Hat ein Use Case mehrere Akteure, so führen diese ihn gemeinsam aus
   * Soll ein Use Case von unterschiedlichen Akteuren jeweils alleine ausgeführt werden, so erstellt man einen generalisierten Akteur.
* So abstrakt wie möglich und konkret wie nötig
* Use Cases nicht zu klein gestalten (Button drücken, Name eingeben)
* Use Cases nicht zu groß gestalten
