---
title: "Vorlesung 5: OOA/OOD mit UML-Diagrammen"
date: "14/11/2017"
---

## Vorlesung 5: OOA/OOD mit UML-Diagrammen

### Modelle und UML-Diagramme
Mit UML lassen sich Software-Systeme modellieren und darstellen. Diese Modelle und Darstellungen lassen sich wie folgt unterteilen:
* __Funktionale Modellierung__
	* Menge von Funktionen, Anwendungsfällen und Diensten
* __Prozessorientierte Darstellung__
	* Menge von Prozessen, Abläufen, Vorgängen und Workflows
* __Daten und Objekt Darstellung__
	* Beziehungen untereinander und Strukturen 

Ein Softwaresystem soll immer in solche Subsysteme zerlegt werden und anschließend aus unabhängigen Komponenten bestehen.

Außerdem gibt es noch die Unterscheidung von __statischen__ und __dynamischen__ Modellen, die in den folgenden Grafiken veranschaulicht wird.
![Pyramide](images/Pyramide.png)

![Pyramide](images/Pyramide2.PNG)
Die Diagramme verfeinern sich von oben nach unten und lassen sich wie oben erwähnt in statisch und dynamisch einteilen.
* Das __statische Modell__ stellt eine allgemeine Gesamtansicht auf ein Problemfeld dar
* Das __dynamische Modell__ stellt Systemverhalten, zeitliche Abläufe, Zustände und Übergänge dar

Im folgendem werden die _wichtigsten_ Diagramme erklärt:
* __Use-Case__(Anwendungsfall)
	* beschreibt Anforderung
	* Außensicht auf das Produkt
	* Testgrundlagen
<img src="images/Usecase.png" alt="Usecase" style="width: 200px;"/>

* __Dynamisches Aktivitätsdiagramm__
	* beschreibt einen Workflow/Szenario
	* Klassen,Objekte und Beziehungen lassen sich hieraus extrahieren
<img src="images/Aktivitätsdiagramm.png" alt="Aktivitätsdiagramm" style="width: 200px;"/>

* __Statisches Paketdiagramm__
	* besteht aus zusammenhängenden Klassen
	* verständlich ohne tiefgehende Untersuchung der Klassen

* __Paket- und Klassendiagramm__
	* guter Überblick über die Ergebnisse des statischen Software-Entwurfs
<img src="images/Packetdiagramm.png" alt="Paketdiagramm" style="width: 200px;"/>
<img src="images/Klassendiagramm.png" alt="Klassendiagramm" style="width: 200px;"/>

* __Sequenz- und Kommunikationsdiagramm__
	* sind dynamisch 
	* beschreibt den Nachrichtenaustausch in einem System
	* Verhalten steht im Vordergrund
<img src="images/Squenzdiagramm.png" alt="Sequenzdiagramm" style="width: 200px;"/>
<img src="images/Kommunikationsdiagramm.png" alt="Kommunikationsdiagramm" style="width: 200px;"/>

* __Zustandsübergangsdiagramm__
	* sehr kleinteilig
	* beschreibt Zustand eines Objekts im Verlauf
	* gut zum Ermitteln neuer Attribute und Methoden
<img src="images/Zustandsdiagramm.png" alt="Sequenzdiagramm" style="width: 200px;"/>




