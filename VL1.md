---
title: "Vorlesung 1: Einleitung"
author: "Jonas Posselt"
date: "21/10/2017"
---

## Vorlesung 1: Einleitung

### Begriffe/Lernziele
**„Software Engineering“ = „Softwaretechnik“**

Lernziel für heute:
* Verstehen, warum Software schwer zu entwickeln ist
* Erklären können, warum Softwaretechnik notwendig ist
* Unterschiedliche <span style="color:red">Arten von Software</span> kennen
* Wissen, welche <span style="color:red">typischen Phasen</span> in einem Softwareprojekt existieren
* Verständnis für <span style="color:red">Rollen</span> in einem Softwareprojekt entwickeln
* Verstehen, dass zur Softwareentwicklung mehr gehört als die reine Programmierung

### Was ist Software?

Der Begriff Software ist weitreichender als das deutsche „Programm“, da zu einer Software auch 
die Dokumentation und alle nötigen Elemente, die für den Betrieb notwendig sind, gehören, wie 
zum Beispiel Datenbankskripte und Betriebshandbücher. Man kann sich einen Eisberg vorstellen u
nd in der Spitze, dem sichtbaren Teil, steht „Software“. Alles was unter dem Wasser liegt gehört 
aber auch dazu.  
Kurz erklärt besteht eine Software aus Programmen, zugehörigen Daten und Dokumentationen, die 
gemeinsam, mit Hilfe eines Computers, Aufgaben erledigen.  
Eine Software besteht aus zwei Teilen, dem Softwaresystem und dem -produkt. Das System ist der 
Kern oder das Herz der Software, also der Teil, den ein Entwickler sieht. Das Produkt ist die 
Schale, oder äußere Schicht, die für den Nutzer erstellt wurde, um den Kern nutzen zu können.  
Es gibt verschiedene Arten von Software. Alles beginnt bei der Systemsoftware, auch dem Betriebssystem 
genannt. Es ist die Schnittstelle zwischen Hard- und Software. Darüber kommen die eingebetteten Systeme, 
die Geräte steuern, um zum Beispiel einen Drucker oder Monitor zu nutzen. Dann gibt es Anwendungssoftware, 
wie Office oder andere Büroanwendungen. Es gibt Standardsoftware, die für jeden Kunden individuell 
angepasst werden kann, darunter Fallen Programme wie SAP. Als letzte Kundensoftware haben wir individuelle 
Software, die extra für einen Kunden entwickelt wurde. Sie wird exakt auf Bedürfnis und Anspruch 
angepasst, ist aber auch dementsprechend teuer, durch sehr zeitaufwändige Entwicklung. Klassisches 
Beispiel wäre eine Software zur Unterstützung spezieller Geschäftsprozesse. Zum Schluss gibt es noch 
Echtzeitsysteme, die man in Flugzeugen, Kraftwerken und Krankenhäusern findet und Informationssysteme, 
die meist aus webbasierten Datenbanken bestehen.  
Da Software immateriell ist kann man den Entwicklungsfortschritt nicht objektiv messen. Dafür verschleißt 
sie nicht. Aber auch Software erreicht irgendwann einen Zeitpunkt, an dem sie ausgetauscht oder 
erneuert werden muss. Diese Alterung kommt von stetiger Änderung im Einsatzgebiet und muss sich an 
diese Änderungen anpassen.


### Software Projekte
**Was ist ein Projekt?**

Ein Projekt ist ein <span style="color:red">Vorhaben</span>, das im wesentlichen durch die <span style="color:red">Einmaligkeit der Bedingungen in ihrer Gesamtheit</span> gekennzeichnet ist, wie z.B.
* Zielvorgabe
* Zeitliche, finanzielle, personelle oder andere Begrenzungen

| Projektgröße | Kriterien | Beispiele |
|:------------ |:--------- |:--------- |
| Light | Bis 6 Personen<br>0-8 Personen-Monate (PM)<br>Technologien: <5 | Rechenprobleme, Alogithmen|
| Medium | 10-30 Personen<br>9-24 PM<br>Technologien: 5-12 | Buchhaltung, Lagerverwaltung |
| Heavy | 50-100 Personen<br>25-45 PM<br>Technologien: 12-20 | Compiler, Datenbank |
| Super Heavy | >100 Personen<br> >45 PM<br>Technologien: >20 | Raumfahrt, Atomkraftwerk, elektronische Börse|

### Klassischer Software Lebenszyklus

Der klassische Software Lebenszyklus besteht aus <span style="color:red">7 Phasen</span>. 

| Phasen | Ergebnisse |
|:------ |:---------- |
| Problem | |
| Requirements Engineering | Anforderungsspezifikation |
| Systemanalyse | Systemmodell |
| Softwareentwurf | Entwurfsspezifikation |
| Implementierung | Entwickelte Software |
| Test | Testdokumentation |
| Wartung & Weiterentwicklung | Betriebsbereite Software |

#### Phasen eines Vorgehensmodells

##### Prozessmanagement
Wie organisiert man die Arbeit einer Softwareabteilung, um regelmäßig kostengünstige und hochwertige Resultate termingerecht zu erzielen?

##### Anforderungsermittlung
Wie findet man heraus, welche Eigenschaften (insbesondere Funktionalität) die zu konstruierende Software haben soll?

##### Analyse
Wie beschreibt man dann diese Eigenschaften?

##### Entwurf
Wie strukturiert man die Software so, dass sie sich leicht bauen und flexibel verändern lässt?

##### Implementierung
Wie realisiert man effizient und fehlerfrei die Software?

##### Wartung
Wie verändert man Software, die keine solche Struktur hat oder deren Struktur man nicht (mehr) versteht?

##### Test
Wie vermeidet man Mängel in Software oder deckt sie auf?

### Rollen in der Softwareentwicklung

#### Begriff
* Eine Rolle beschreibt eine Menge von zusammengehörigen Aufgaben und Befugnissen (oft auch notwendige Qualiﬁkationen)
* Eine Rolle wird von einer oder mehreren Personen wahrgenommen
* Eine Person kann mehrere Rollen einnehmen
* Nicht in jeder Softwareentwicklung treten alle Rollen auf, abhängig von Art und Größe des Projekts

#### Ziel
* Kooperation zwischen den beteiligten Personen durch Verständnis für die Aufgaben

#### Akteure
| Akteur | Aufgabe |
|:------ |:---------- |
| Auftraggeber | Bezahlen das Projekt, haben unterschiedliche Bedürfnisse |
| Benutzer | Benutzen die Software</br>Manchmal mit Auftraggeber identisch |
| Manager | Treffen während der Entwicklung die organisatorischen Entscheidungen |
| Berater | Unterstützen den Kunden in der Definition der Anforderungen |
| Entwickler | Definieren und entwickeln Software</br>in verschiedenen Rollen aufgeteilt(d.h. mit verschiedenartigen Aufgaben)|

#### Rollen bei der Auftragsarbeit
Ein Manager gibt einen Auftrag an ein Auftraggeber, diese Person bespricht den Auftrag mit einem Fachexperten und einem Jurist.</br> Der Auftraggeber sucht sich ein Unternehmen oder eine einzelne Person, der sogenannte Auftragnehmer, mit der wird der Auftrag besprochen.</br> Der Auftragnehmer bespricht den Auftrag ebenfalls mit einem Juristen und einem Computerspezialist. Nach der Besprechung gibt er den Auftrag an einen Projektleiter, dieser kümmert sich dann um das gewünschte Projekt. </br>
Rücksprache gibt es weiterhin unter den ganzen Beteiligten. 

#### Typische Rollen 
[Siehe auch](#/VL1?id=rollen-aus-informatik-perspektive)

* Technischer Projektleiter
* Kaufmännischer Projektleiter
* Analytiker
* Entwickler
* Konfigurationmanger
* Sicherheitsexperte
* Softwarearchitekt
* Tester 
* Qualitätmanager

### Rollen aus Informatik-Perspektive

| Rolle | Aufgaben/Ziele | Aktivitäten |
|:----- |:-------------- |:----------- |
| Projektmanager | erfolgreiche Projektdurchführung | <ul><li>Planung des Projekts: Projektorganisation; Kostenschätzung und Planung; Erstellung eines Projektplans</li><li>Kontrolle des Projekts: Produktverfolgung; Planüberprüfung; Produktivitätsüberwachung</li><li>Steuerung des Projekts: Projektkoordination</li></ul> |
| Anforderungsanalytiker | Aufnahme und Überprüfung von Anforderungen an das System<br>„Was“ soll das System leisten? | <ul><li>Ermitteln und Erkennen von Benutzer-Anforderungen: „Was macht das derzeitige System“; Ist-Analyse; Soll- Analyse: „Was soll das zukünftige System tun“ </li><li>Machbarkeitsstudie: Bewertung der Ist- und Soll-Analyseergebnisse</li><li>Integration unterschiedlicher Sichten/Ziele: Kommunikation mit Anwendern, Kunden etc. und Übereinstimmung der Beteiligten bzgl. der definierten Anforderungen</li><li>Erstellung eines Anforderungsdokuments</li></ul> |
| Software-Architekt | Architektur des Systems<br>Übergang vom Problem zur Realisierung („Wie“) | <ul><li>Zuordnung von Anforderungen auf Komponente/Subsysteme</li><li>Grobentwurf: Subsysteme, evtl. grobgranulare Komponenten und deren Beziehungen</li><li>Sicherstellung von Qualitätsattributen (Struktur des Systems beeinflusst Qualitätsattribute)</li><li>Dokumentation der Systemarchitektur</li></ul> |
| Software-Designer | Beschreibung des Verhaltens, der Daten und der Funktionen des Systems<br>Entwurf einer „implementierungsnahen“ Speziﬁkation des Softwaresystems („technische Anforderungen“) | <ul><li>Modellierung/ Beschreibung der Anforderungen aus „Implementierungssicht“  (Kommunikation mit Architekt und Programmierer)</li><li>Feinentwurf: Detaillierter Entwurf des Systems (Komponenten, Interfaces, Klassen)</li></ul>|
| Programmierer/Entwickler | programmiertechnische Umsetzung (Realisierung, Implementierung) des Entwurfs | <ul><li>Programmierung der einzelnen Komponenten</li><li>Dokumentation des Programmcodes</li><li>Definition der spezifischen Algorithmen</li><li>Beachtung von Standards</li><li>Entwickler-Test der Module (z.B. JUnit-Tests)</li><li>Code-Reviews</li></ul> |
| Tester | führt das System aus, um Hinweise auf Fehler zu ﬁnden (Systemtests, Integrationstests)<br>Abwesenheit von Fehlern kann durch Testen **NICHT** garantiert werden | <ul><li>Detaillierung von Testplan, Testentwurf und Testfällen</li><li>Durchführung von Tests (Dokumentation der Testbedingungen und Testergebnissen)</li><li>Überprüfung der Zusammenarbeit der Komponenten</li><li>Überprüfung des Gesamtsystems</li></ul> |
| Konfigurationsmanager | Festlegung der Regelungen für Konfigurations- und Produktverwaltung | <ul><li>Überwachung der Konfiguration des Produkts Konfigurationskontrolle und Statusverfolgung</li><li>Nachvollziehbarkeit und Konsistenz: Sicherstellung von Sichtbarkeit, Verfolgbarkeit und Kontrollierbarkeit eines Produkts und seiner Teile im Lebenszyklus</li></ul> |
| Administrator | Betrieb des Softwaresystems | <ul><li>Installation der Software</li><li>Überwachung des laufenden Software durch Monitoring von Log-Files</li><li>Einspielen von Software-Updates</li></ul> |

Weitere Rollen ([Quelle](http://dewik.de/content/SE_Zusammenfassung_Kap_4_7.pdf "Kapitel 4: Rollen in der Software Engineerings")):
* Risikomanager
* Qualitätsmanager
* Spezifizierer
* Systemtechniker
* Technologieberater
* Wartungsexperte
* Datensammler- und bewerter
* Software-Prozessverbesserer
* Wiederverwender

### Unterschiedliche Projektgrößen

**Entwicklung von kleinen / großen Softwaresystem**

* die Herstellung großer Software unterscheidet sich qualitativ und quantitativ im Vergleich zu kleinen Softwaresystemen
* die Komplexität von großen Softwaresystemen kann die Kapazitäten des Entwicklers übersteigen
* ein System aus vielen Modulen ist Fehleranfälliger als die Module selbst
* die Langlebigkeit und Versionierung großer Softwaresysteme ist problematisch
* die Kommunikation zwischen den beteiligten Personen ist schwierig

| Projektgröße | Rollen | Warum? |
|:-------------|:-------|:-------|
| Light | Kunde, Management,<br>Programmierer, Tester | Besteht meistens aus nur<br>einer Person die alle Rollen<br>in sich vereint.|
| Medium | Kunde, Projektleiter, Analytiker,<br>Programmierer, Tester, Controller | Projekt umfangreicher<br>Zusammenarbeit mehrerer<br>Personen notwendig |
| (Super) Heavy | Kunde, Management, wirschaftlicher<br>und technischer Projektleiter,<br>Gruppenleiterm Analytiker, Controller,<br>Programmierer, Tester,<br>Qualitätssicherer | Projekt für Einzelne nicht<br>mehr überschaubar,<br>Aufteilung in Gruppen mit<br>Struktur des Ganzen |

### Software Qualität

### Probleme in der Software Entwicklung

### Softwarekosten

* Wartung ist teurer als die Entwicklung
* Test- und Entwicklungskosten sind fast gleich hoch
* Typ und Anforderungen wie Performance und Systemzuverlässigkeit beeinflussen die Kosten des Systems
* die Verteilung der Kosten ist abhängig vom verwendeten Vorgehensmodell
* der größere Teil der Entwickler arbeiten an der Pflege der Software

**Fehlerentstehung und -erkennung**

Die Fehler entstehen nur in den ersten drei Phasen: Analyse, Design und Implementierung, wobei 90% der Fehler im Design und der Implementierung entstehen. Dennoch werden die meisten Fehler erst währen den Modul- und Systemtests gefunden.
Dies ist problematisch, da die Kosten zur Behebung der Fehler mit jedem weiteren Schritt steigen. Die Beseitigung von Fehlern betragen zwischen 30%-60% wenn man sie in den Tests findet und 100% wenn das System im Einsatz ist.

Bei einem Projekt, bei dem mehr als eine Person die Software entwickelt, entstehen mehr als eine Version der Software. Software Engineering hilft dabei, dass Fehler nicht entstehen oder die zu beseitigen.

###Was ist Software Engineering?

Software Engineering ist ein Teilgebiet der praktischen Informatik, die das Software Management, die Entwicklung und Qualitätssicherung zusammenfasst.
Weitere Themen die unter Software Engineering fallen sind: Software...
* ... Requirements
* ... Design
* ... Construction
* ... Testing
* ... Quality
* ... Maintenance
* ... Engineering Tools & Methods
* ... Configuration Management
* ... Engineering Process

Durch Software Engineering und die Verwendung von Methoden, Werkzeugen und Vorgehensmodellen werden die Kosten, die bei der Entwicklung, Wartung und Erweiterung anfallen, reduziert mit der Erhaltung von hoher Qualität.

**Ziele des Software Engineerings**
* Schnelle und effiziente Entwicklung des Produkts (Entwicklungsaspekt)
* Einhaltung der geforderten Qualitätsmerkmale (Qualitätssicherungsaspekt)
* Kontrollierte Projektabwicklung (Managementaspekt)
* Sicherstellung der Wartbarkeit, Erweiterbarkeit, Wiederverwendbarkeit (Wartungsaspekt)

Insgesamt steht die Qualität im Mittelpunkt, es wird mit (agilen) Vorgehensmodellen gearbeitet, die Entwicklung wird methodisch durchgeführt und es werden Softwarewerkzeuge zur Beherrschung der Komplexität benutzt.

### Zusammenfassung
* Software Engineering ist eine <span style="color:red">Ingenieur-Disziplin</span>, die sich mit allen Aspekten der Softwareentwicklung und Softwarewartung beschäftigt.
* Ziel des Software Engineerings ist die Erreichung einer <span style="color:red">hohen Softwarequalität</span> und die <span style="color:red">Minimierung der Softwarekosten</span>.
* Software Engineering ist mehr als Technik und befasst sich mit <span style="color:red">Konzepten, Methoden und Werkzeugen</span> für die professionelle Softwareentwicklung
* Softwareprodukte bestehen aus <span style="color:red">Programmen und der Dokumentation</span>
* Software Ingenieure arbeiten in <span style="color:red">Teams</span> in Software Projekten methodisch und strukturiert und <span style="color:red">kommunizieren</span> mit Kunden und Teammitgliedern
* Software Ingenieure beherrschen die Technik und lassen sich nicht von der Technik beherrschen
* Der <span style="color:red">Softwareentwicklungsprozess besteht aus Phasen</span>, die bei der Entwicklung des Softwareprodukts involviert sind. Die grundlegenden Phasen sind <span style="color:red">*Analyse, Entwurf, Implementierung, Integration, Test, Wartung und Weiterentwicklung*</span>.