## Vorlesung 8: Systemanalyse mit Analyseklassendiagrammen

### Lernziele

- Klassendiagramme mit UML modellieren können
- Analyseklassendiagramme aus Anforderungen ableiten können
- Ermitteln von Klassen, Attributen und Beziehungen fürAnalyseklassendiagramme

### Klassendiagramme
<center>
![Klassendiagramm](./images/VL08/Klassendiagramm.png)
</center>

#### Sichtbarkeit
Definiert die Sichtbarkeit des Attributes fürandere Elemente
<center>
![Sichtbarkeit](./images/VL08/Sichtbarkeit.png)
</center>

<center>
![Abgeleitete Attribute](./images/VL08/AbgeleiteteAttribute.png)
</center>

- Beispielfür berechnetes Attribut: Klasse mit Attribut für Preis. Abgeleitetes Attribut: Preis mit Mehrwertsteuer.
- Keine Angabe der Sichtbarkeit = default. Default = package.
- Statische Attribute & Methoden sind unterstrichen
- Abstrakte Methoden und Klassen sind kursiv

#### Generalisierung und Spezialisierung
<center>
![Generalisierung](./images/VL08/Generalisierung01.png)
</center>

<span style="color:red">**Hinweis:**</span> Mehrfacherbung ist in UML zulässig

<center>
![Generalisierung](./images/VL08/Generalisierung02.png)
</center>

#### Stereotypen
- Ein Stereotypklassifiziert Modellelemente wie Klassen oder Attribute.
- Durch einen Stereotyp wird die Bedeutung des  Modellelements spezialisiert  und kann so beispielsweise bei der Codegenerierung spezifischer behandelt werden.

<center>
![Stereotypen](./images/VL08/Stereotypen01.png)
</center>

<center>
![Stereotypen](./images/VL08/Stereotypen02.png)
</center>

#### Merkmale
- Ein Merkmal wird normalerweise in der Form {name = wert} notiert
- {abstract} = {abstract = true}
- Eigene Merkmale können für Klassen und Attribute definiert werden

<center>
![Merkmale](./images/VL08/Merkmale.png)
</center>

#### Verantwortlichkeiten
- Ein Vertrag oder eine Verpflichtung einer Klasse, einen bestimmten Dienst auszuführen
- Verantwortlichkeiten stehen im Klassendiagramm bei einer Klasse unter den Operationen
- Werden selten verwendet

<center>
<img src="images/VL08/Verantwortlichkeiten.png" alt="Verantwortlichkeiten" width="300"/>
</center>

### Assoziationen

### Logisch-statische Sicht auf ein Softwaresystem mit Analyseklassendiagrammen in der Systemanalyse

### Best Practices

### Beispiel