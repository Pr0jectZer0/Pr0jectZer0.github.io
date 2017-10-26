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

### Rollen in der Softwareentwicklung

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
