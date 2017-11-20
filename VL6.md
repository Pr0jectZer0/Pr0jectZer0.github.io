---
title: "Vorlesung 6: Anforderungsanalyse"
date: "20/11/2017"
---

## Anforderungsanalyse

### Satzschablonen für die Anforderungsermittlung

#### Visualisierung der Systemaktivitäten
<center>
![OOD](/images/visualisierungsystemaktivitaeten.png)
</center>

#### Charakterisierung der Systemaktivitäten
1. Selbstständige Systemaktivität
  Das System **führt** den Prozess selbstständig durch.
2. Benutzerinteraktion
  Das System **stellt** dem Nutzer die Prozessfunktionalität zur Verfügung.
3. Schnittstellenanforderung:
  Das System führt einen Prozess in Abhängigkeit von einem Dritten (zum Beispiel einem Fremdsystem) aus, ist an sich passiv und wartet auf ein externes Ereignis.

#### Satzschablone nach Rupp
<center>
![OOD](/images/satzschablone.png)
</center>

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

<center>
![OOD](/images/if.png)
</center>

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
