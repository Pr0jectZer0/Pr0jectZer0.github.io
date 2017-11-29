# Systemanalyse mit Aktivitaetsdiagrammen

## Grundlagen

<img src="images/VL_07_Entwicklungsprozess.png" width=1000>

<img src="images/VL07_problem_space.png" width=1000>

### Die Anforderungsanalyse
  - beschreibt Anwendungsfälle und Akteure
  - spezifiziert Geschäftsvorfälle mit Text
  - definiert die GUI

### Die Systemanalyse
- detailliertes Verständnis des Softwaresystems -> Probleme entdecken, bevor das System realisiert wird
- untersucht Problemgebiet -> vollständige Formulierung und Verständnis von gewünschtem Verhalten
- präzisiert Anforderungsdefinition -> Herausfinden, was Auftraggeber und Anwender wirklich wollen
    - Aspekte der Implementierung ausgeklammern, klare Trennung zwischen Anforderungen und Umsetzung
          - Betrachtung der reinen Anforderungen (Was will der Benutzer/Auftraggeber tatsächlich?), Untersctellung einer „perfekten Technik“ (keine Performance- oder Speicherbeschränkungen, keine Verteilungsproblematik etc.)
          - Softwareentwurf: Definition der technischen Lösung, Umsetzung der Anforderungen
- Einheitliches Verständnis zwischen Kunden und Entwicklern sowie innerhalb des Entwicklungsteams
- stellt sicher, dass Sachverhalte des Problemgebiets korrekt umgesetzt werden
- beherrscht die Komplexität und entdeckt Gemeinsamkeiten
- Priorisierung der Anforderungen und Entscheidung über ihre Realisierung

#### Die Systemarchitektur als Beispiel für ein Systemanalysemodell
- Die Systemarchitektur anhand von Beschreibungen (Source Code, natürliche Sprache) zu verstehen, ist schwer und kostet Zeit
- Daher wird die Systemarchitektur visuell auf abstraktem Niveau zum Beispiel als Client-Server-Architektur oder als Peer-to-Peer Architektur in Form eines „Box-and-arrows“-Diagramms
<img src="images/VL07_systemarchitektur_beispiel.png" width=1000>
- !!!Benutzen Sie dieselben Symbole für die gleichen Dinge | Fügen Sie eine Legende hinzu!!!

#### Einordnung der Systemanalyse in Analogie zu einem Hausbau
<img src="images/VL07_einordnung_systemanalyse.png" width=1000>
- Das Wesentliche einer (Software)-Architektur lässt sich in der Regel nicht in einer Sicht allein darstellen, sondern man verwendet verschiedene Sichten
- Für ein konkretes Softwaresystem wählt man „passende“ Sichten, um die Architektur darzustellen.
- Die Architekturdokumentation hilft anderen und auch einem selbst, eine Software-Architektur zu verstehen und zu analysieren
- In folgenden Projekten wird Wissen über den Architekturentwurf weitergegeben
- Eine Methode, Softwarearchitektur darzustellen, ist über die objektorientierte Analyse mit UML-Diagrammen 

#### UML-Modelle in der Objektorientierten Systemanalyse
- Ausgangspunkt der OOA ist die Anforderungsdefinition (insbesondere Use Cases)
- Bestandteil des OOA-Modells ist das Analyseklassendiagramm (Domain Object Model)
    - Vollständige Darstellung der fachlichen Daten-Anforderungen an das System
    - Ausgangsmodell für die Entwicklung des OOD-Klassendiagramms
- Ausgangspunkt der Aktivitätsdiagramme sind Use Case-Diagramme und textuelle Use Case–Beschreibungen
- Textuelle Use Cases Definitionen werden mittels Aktivitätsdiagrammen visualisiert  
    - Sie dienen auch der Spezifikation von Testfällen und damit zur Systemvalidierung
- Spezifikation der zeitlich-logische Abläufe (z.B. Geschäftsvorfälle) mit Aktivitätsdiagrammen zur Beschreibung der dynamischen Aspekte
- Mögliche Einsatzgebiete von Aktivitätsdiagrammen sind 
    - die Beschreibung Use Case-übergreifender Abläufe
    - die Spezifikation des Ablaufs innerhalb eines Use Cases
    - die Dokumentation des Kontrollflusses einer Operation
  
## Aktivitätsdiagramme
### Aufgaben, Zwecke und Einsatzgebiete von Aktivitätsdiagrammen
- Visualisierung von Use Cases zur Verbesserung des Verständnisses und der Analyse des Ablaufs von komplexen Szenarios 
- Modellierung von Abläufen Datenflüssen in einem System
- Generierung von Testfällen
- Dienen auch zur Geschäftsprozessmodellierung 
- Darstellung übergreifender Abläufe über Use Cases hinweg (Geschäftsvorfall)
- Es können sowohl sequentielle als auch parallele Abläufe modelliert werden
- Darstellung von zeitlich-logischen Abläufen in Form von aufeinanderfolgenden Aktivitäten inklusive Verzweigungen und parallelen Vorgängen
- Algorithmus einer Operation
<img src="images/VL07_UseCase.png" width=1000>

#### Zu jedem Use Case genau ein Aktivitätsdiagramm modellieren
- Erzeugen Sie aus den Use Case-Schritten Aktionen.
- Zerlegen Sie die Aktionen ggfs. mit einem Aktivitätsdiagramm, so dass sie stets genau einen fachlichen Arbeitsschritt repräsentieren.
- Ergänzen Sie den Ablauf um alle bekannten fachlichen Ausnahmen und fachlichen Ablaufvarianten, so dass das Diagramm eine vollständige Beschreibung aller zulässigen Ablaufmöglichkeiten darstellt.
#### Modellierung des Objektflusses
- Beschreiben Sie zu jeder Aktion die zu verarbeitenden und die resultierenden  Geschäftsobjekte.
- Beschreiben Sie, bei welchen ausgehenden Transitionen bzw. Bedingungen welche Objekte bzw. Objektzustände resultieren.

## Notationselemente für Aktivitätsdiagramme
<img src="images/VL07_aktivitätsdiagramm_01.png" width=1000>
<img src="images/VL07_aktivitätsdiagramm_02.png" width=1000>
<img src="images/VL07_aktivitätsdiagramm_03.png" width=1000>
<img src="images/VL07_aktivitätsdiagramm_04.png" width=1000>
## Aktivitätsdiagramme Beispiele

## Best Practices

## Zusammenfassung
