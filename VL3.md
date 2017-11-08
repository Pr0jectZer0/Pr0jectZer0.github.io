## Vorlesung 3: Agile Vorgehensmodelle (XP, Scrum, Kanban)

### (e)Xtreme Programming (XP)
XP ist ein Vorgehensmodell welches darauf basiert viele kleine Inkremente zu entwickeln und auszuliefern, weshalb es eine Weiterentwicklung der Inkremetellen Entwicklung ist. Es wird sich auf aktuelle Probleme konzentriert und probiert den einfachsten Entwurf der möglich ist zu entwickeln. Dabei wird davon ausgegangen dass der Kunde die Anforderungen an die Software zu Projektbeginn nicht komplett kennt. Auch ein Grund dafür, dass Teamarbeit und Offenheit im Vordergrund stehen und Kommunikation eine Grundsäule im Vorgehensmodell ist. XP soll Vorteile bringen, wie dass die Software schneller bereitgestellt werden kann und die Softwarequalität sowie die Zuffriedenheit des Kunden soll deutlich besser als bei herkömmlichen Ansätzen sein. Der Kunde soll aktiv am Herstellungsprozess beteiligt werden. 

### XP Paarprogrammierung
Bei der XP Paarprogrammierung arbeiten jeweils 2 Programmierer an einer Maus und einer Tastatur und jede Programmiertätigkeit wird im Paar ausgeführt. Während der eine Maus und Tastatur bedient und den Code schreibt, Kontrolliert der andere den geschriebenen Code, denkt über die Problemstellung nach und spricht Probleme, die ihm auffallen sofort an. Diese Methode soll zu einem Qualitativ hochwertigerem Programmtext führen, doch auch der Nachteil für Unternehmen ist deutlich: Doppelte Personalkosten.

### „Test first“ und Test-driven-development (TDD)
**(Testgetriebene Entwicklung)**
Die Testgetriebene Entwicklung ist ein Desingmuster bei dem zu aller erst Tests geschrieben werden die erstmal fehlschlagen und erst anschließend den Code der getestet werden soll. Allerdings nur genau so viel Code, dass der Test erfolgreich durchläuft. Falls mehr Code geschrieben wird entstehen nicht getestete stellen die im nächsten Schritt, bei Refactoring Probleme machen könnten. Beim Refactoring sollen Tests und Programmcode gleichermaßen aufgeräumt werden. Die drei Schritte werden Zyklisch durchgeführt. Das Vorgehen hilft Mehrdeutigkeiten oder Lücken in den Spezifikationen besser zu erkennen, bringt Testautomatisierung und Kompensiert eine Fehlende Entwurfsphase.

![Test Code Refactor Zyklus](/images/testcoderefactor.jpg "Test Code Refactor Zyklus")

### Scrum (Rollen)

**Product Owner:**
Beim Scrum Modell gibt es drei Rollen wobei der Product Owner beispielsweise der Auftraggeber ist, also derjenige der die Anforderungen und die Deadline festlegt, sowie das Budget bereitstellt. Außerdem hat der Owner die Aufgabe das Product-Backlog zu führen in dem er seine Vorstellungen von der weiteren Entwicklung aufnehmen soll. Dort werden Anforderungen Priorisiert und angepasst.

**Scrum Master:**
Der Scrum Master arbeitet eng mit dem Product Owner zusammen, sorgt dafür, dass sich an die Scrum-Werte und Techniken gehalten wird, hilft die Produktivität des Teams zu steigern und Eliminiert Störungen. Er Moderiert außerdem die Meetings, hilft bei der Vorbereitung und soll das Team voranbringen indem er Hindernisse beseitigt und die Zusammenarbeit aller Rollen unterstützt.

**Scrum Team (Entwicklungsteam):**
 Das Entwicklungsteam (5-9 Personen) sind Personen mit verschiedenem Fachwissen. Das Team besitzt alle Qualifikationen um die Anforderungen zu Implementieren. Es werden keine Aufgaben zugewiesen, sondern Mitglieder übernehmen diese. In einem Sprint können sich die Mitglieder des Teams nicht ändern.

### Product Backlog (Anforderungsliste)

Der Produkt-Owner soll das Backlog führen indem die Eigenschaften des Produkts priorisiert aufgelistet werden. Höher priorisierte Einträge sind detaillierter dargestellt. Das Product Backlog ist Sichtbar für alle und alle können Einträge beisteuern. Die Anforderungen werden nach absteigender Priorität abgearbeitet.

### Scrum Konzept 
* Das Entwicklungsteam wählt die Anforderungen aus den Produktanforderungen aus, die es in diesem Sprint erledigen kann und erstellt zusammen mit dem Scrum Master das Sprint Backlog (Aufgabenliste).
* Ort und Zeit des täglichen Scrum Meeting wird festgelegt
* Start- und End- Datum wird festgelegt, meist 30 Tage.
* Das Team wählt Einheiten, zu deren Implementierung es sich verpflichten kann, aus dem Product Backlog aus
* Tasks werden identifiziert und geschätzt (1-16 Stunden)

#### Schätztechniken
* Teilziele innerhalb des Produkt- bzw. Sprint-Backlog sind zu schätzen
* Geschätzt wird in abstrakten, vergleichenden „Story-Punkten“
* Jedes Teammitglied schätzt aufgrund seiner bisherigen Geschwindigkeit und es wird ein Mittelwert gebildet 
* Bei umfangreichen Anforderungen, sollte nach Möglichkeit eine Aufteilung und Re-Priorisierung in Betracht gezogen werden, da kleinere und mittelgroße Anforderungen leichter zu planen und schneller umzusetzen sind.

#### Daily Scrum (tägliches Scrum-Treffen)
* Täglich, derselbe Ort und die Gleiche Zeit, ca 15 Minuten
* Dient der Selbstorganisation des Teams
* Jedes Team Mitglied beantwortet 3 Fragen
** Was hast du seit dem letzten Mal geschafft?
** Was wirst du bis zum nächsten Mal tun?
** Was behindert dich beim Vorwärtskommen
* Weiterführende Diskussionen werden im Anschluss geführt
* Alle sind eingeladen, aber nur Team-Mitglieder und der Scrum-Master dürfen reden. Die Hindernisliste wird ggfs. Aufgefüllt
* Das Meeting beginnt mit dem Check, ob das Team die Ziele, vom letzten Meeting erreicht hat und der Zeitplan eingehalten werden kann.

#### Sprint
* Serien von Sprints bringen ein Scrum-Projekt iterativ voran
* Das Produkt wird während des Sprints entworfen, kodiert und getestet
* Am Ende steht ein auslieferbares Stück Software
* Keine Änderungen der Anforderungen während des Sprints

#### Sprint-Review-Treffen
* Das Entwicklungsteam stellt die Ergebnisse des Sprints vor, z.B. in Form einer Demonstration der neuen Features.
* Es werden keine Folien verwendet, sondern es wird typischerweise eine Software Demo präsentiert
* Das gesamte Team präsentiert, was es während eines Sprints erreicht hat
* Der Product Owner und andere geben Feedback
* Abnehmen kann der Product Owner nur Anforderungen, die bis zum Sprint-Review vollständig und fehlerfrei umgesetzt sind. 
* Angefangene, aber nicht abgeschlossene Arbeiten werden als nicht erledigt gewertet. Beim Sprint-Review mit seinem Check-Charakter wird in besonderem Maße sichtbar, was bereits erarbeitet wurde und wo möglicherweise noch Anpassungsbedarf besteht.

#### Sprint-Retrospektive
* Der zurückliegende Sprint wird analysiert
* Teilnehmer sind das Entwicklungsteam, der Scrum Master, der Auftraggeber sowie evtl. der Endkunde
* Was lief gut während des Sprints?
* Was kann im nächsten Sprint verbessert werden?
* Diskussion der identifizierten Probleme

### User Stories
Eine User-Story ist eine in Alltagssprache formulierte Software-Anforderung, die vom Benutzer oder Entwickler kommen kann. Sie ist bewusst kurz gehalten und umfasst in der Regel nicht mehr als zwei Sätze. Ein Beispiel wäre:
> Als Vertragshändler möchte ich alle Gebrauchtwagen auflisten können, um diese meinen Kunden anzubieten.

Aus User Stories können Akzeptanzkriterien abgeleitet werden, die Beispielsweise so aussehen könnten:
> Ein Anmeldeformular ist verfügbar
> Beim Anlegen neuer User werden die Zahlungsdaten abgefragt

User Stories können nach __Zielen__, __MoSCoW-Methode__ oder nach __Kano-Analyse__ priorisiert werden.
Bei der Zielpriorisierung unterscheidet man zwischen __KANN__, __SOLL__, __MUSS__. Wohingegen bei der MoSCoW-Priorisierung noch __WON'T__ hinzukommt.

![MoSCoW-Priorisierung](/images/moscov.png "MoSCoW-Priorisierung")

### Wireframes
Wireframes sind Skizzenähnliche Entwürfe graphischer Benutzeroberflächen. Sie haben keine Farben oder Bilder. Man unterscheidet Wireframes in statischen und dynamischen Wireframes. Bei einem __statischen Wireframe__ handelt es sich um eine schematische Darstellung von nur einer einzelnen Benutzeroberfläche. __Dynamische Wireframes__ bestehen aus mehr als einer Seite. Die einzelnen Seiten werden interaktiv miteinander verknüft und bilden einen funktionellen Prototypen.

![Wireframes](/images/wireframe.jpg "Wireframes")

### Sprint Backlog
Sprint Backlog ist im Grunde eine Aufgabenliste, mit Aufgaben, die zur Erfüllung des Sprint-Zieles notwendig sind.

### Scrum Boards
Das Scrum Board zeigt die Gesamte Aktivität eines Sprints an.

![Scrum Boards](/images/scrumboard.jpg "Scrum Boards")

### Was ist Kanban? 
* Entstammt dem Produktionsbereich von Toyota
* Ziel: Reduzierung der Lagerbestände durch Finden des optimalen Arbeitsflusses („Just-in-time-Produktion“)
* Wird als agiles Vorgehensmodell auch in der Softwareentwicklung verwendet
* Hohe Flexibilität sowie geringe Komplexität
* Prinzip der kontinuierlichen Verbesserung, der bestehende Prozess wird in kleinen Schritten verbessert
* Fördert Transparenz und Kommunikation im Team
* Kanban schreibt nicht vor, wie etwas getan werden soll, sondern nur, dass es getan werden muss.
* Kein Push-, sondern Pull-Prinzip, man sieht was noch zu tun ist
* „Produziere nur das, was benötigt wird, wenn es benötigt wird“
* Mitarbeiter wählen ihre Aufgaben selber zB nach Stärken, Erfahrungen und Einarbeitung

#### Die sechs Kernpraktiken von Kanban
Mache Arbeit sichtbar
* Die Wertschöpfungskette mit ihren verschiedenen Prozessschritten (zum Beispiel Anforderungsdefinition, Programmierung, Dokumentation, Test, Inbetriebnahme) wird gut sichtbar für alle Beteiligten visualisiert.
* Dafür dient das Kanban Board
Limitiere den Work-in-Progress (WiP)
* Die Anzahl der Tickets (Work in Progress – WiP), die gleichzeitig an einer Station bearbeitet werden dürfen, wird limitiert. Wenn beispielsweise die Programmierung gerade zwei Tickets bearbeitet, und das Limit für diese Station zwei beträgt, darf sie kein drittes Ticket annehmen, auch wenn die Anforderungsdefinition ein weiteres bereitstellen könnte. Hierdurch entsteht ein Pull-System, bei dem sich jede Station ihre Arbeit bei der Vorgängerstation abholt, anstatt fertige Arbeit einfach an die nächste Station zu übergeben.
Kontrolliere den Arbeitsfluss
Mache die Prozessregeln explizit
* Man muss explizit sich auf Sachen einigen, zB wie der Begriff ‚fertig‘ definiert wird.
Implementiere Feedback-Mechanismen
* Verbesserung entsteht nur wenn sich alle Ebenen in der Organisation daran beteiligen.
Führe gemeinschaftliche Verbesserungen durch

#### Mache Arbeit sichtbar
* Der gesamte Prozess wird am Kanban-Board dargestellt
* Durch die Visualisierung werden Fehler, Problemquellen und Engpässe leichter gefunden

![board](/images/board.png)
	
#### Das Kanban-Board
* Behindern Limitierungen den Arbeitsfluss?
* Probleme beim Release legen den ganzen Betrieb lahm
* Oft ist es besser, den Betrieb erst fortzusetzen, wenn der Engpass behoben ist

#### Limitiere den Work-in-Progress (WiP) sequentielle versus parallele Arbeit

![arbeit](/images/arbeit.png)

* Menschen sind von Natur aus nicht multitaskingfähig
* Das Wechseln zwischen Tätigkeiten erfordert Einarbeitungsaufwand
* Beispiel: Programmierer wird ständig durch Zwischenfälle von seiner Hauptaufgabe abgelenkt
* „Eine zu 100% abgeschlossene Aufgabe ist besser als zehn zu 10% abgeschlossene Aufgaben.“

### #2: Limitiere den Work-in-Progress (WiP)
Obwohl parallele Arbeit langsamer ist, geht es nicht Ohne. Deswegen muss die Anzahl an paralleler Tätigkeiten limitiert werden.  Das bring eine Höhere Effizienz, eine bessere Übersicht und weniger Überlastung

### #3: Kontrolliere den Arbeitsfluss
Engpässe behindern den Arbeitsfluss am meisten also gilt es diese zu vermeiden. Teile die Aufgaben in Arbeitstypen und Serviceklassen auf wobei der Arbeitstyp die art der Tätigkeit beschreibt und die Serviceklasse die Klassifizierung von Arbeit nach der Auswirkung auf das Geschäft ist. 

Beispiele für Arbeitstypen (z.B. Visualisierung durch Zeilen) - Neue Features, Bugfix, Wartungsarbeit
Beispiele für Serviceklasse (z.B. Visualisierung durch Farbe der Zettel am Board) - Standard, fester Liefertermin, beschleunigt (= hohe Priorität)
![Arbeitsfluss](/images/arbeitsfluss.jpg "Arbeitsfluss")

### #4: Mache die Prozessregeln explizit
Kanban gibt selbst wenige Regeln vor und die Regel die das Team bestimmt sollten deshalb für jeden einsehbar sein. Beispiele dafür könnten sein: - „Definition of Done“ (ähnlich Scrum) - Was genau bedeuten die einzelnen Spalten?

### #5: Implementiere Feedback-Mechanismen
Kanban hat die stetige Verbesserung durch Kommunikation der Mitarbeiter untereinander als Ziel. Dadurch sollen Schwächen erkannt, Probleme diskutiert und Änderungen beschlossen werden.

**Daily Standup Meetings**
Das Team Trifft sich in täglich sogenannten Daily Standup Meetings, um den Fortschritt zu besprechen. 
**Retrospektive**
Außerdem gibt es ein Meeting  in größeren Abständen zur ausführlichen Besprechung in größeren Abständen. In denen soll aus der Vergangenheit gelernt werden.

**Operations Review**
Damit das Team ein Bild für das große Ganze bekommt gibt es noch eine Besprechung mit Leuten aus anderen Abteilung.

### Kanban und Scrum: Gemeinsamkeiten und Unterschiede
Kanban und Scrum können kombiniert werden und schließen sich nicht gegenseitig aus.

__Gemeinsamkeiten:__
* agil und schlank („lean“)
* setzen auf Transparenz
* fördern Kommunikation und Selbstorganisation im Team
* Pull-System
* brechen große Aufgaben in Teilaufgaben auf
* setzen auf inkrementelle Verbesserungen

__Unterschiede:__
![Scrum Boards](/images/kabanscrum.png "Scrum Boards")

__Vorteile von Scrum:__
* durch feste Rollenverteilung entwickelt sich schneller eine Routine
* auch in größeren Gruppen einsetzbar

__Vorteile von Kanban:__
* mehr Freiheit und weniger Bürokratie