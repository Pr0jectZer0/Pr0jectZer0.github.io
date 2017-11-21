---
title: "Vorlesung 6: Anforderungsanalyse mit UML-Use Case Diagramm, Satzschablone und textueller Use Case Definition"
date: "20/11/2017"
---

## Vorlesung 6: Anforderungsanalyse mit UML-Use Case Diagramm, Satzschablone und textueller Use Case Definition

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
