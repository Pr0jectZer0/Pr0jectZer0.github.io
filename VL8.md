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

#### Arten von Assoziationen

Eine Modellierung der Assoziationen zeigt die Zusammenhänge zwischen Objekten von Klasse. Wichtig dabei ist, dass sich alle Assoziationen 
außer der Vererbung auf Objekte bezieht und nicht auf deren Klassen.

<center>
<img src="images/VL08/Assoziationspfeile.png" alt="Assoziationspfeile" width="600"/>
</center>

#### Navigierbarkeit

Die Art der Assoziation bestimmt die Richtung, in der die Objekte miteinander interagieren.

<center>
<img src="images/VL08/Navigierbarkeit.png" alt="Navigierbarkeit" width="600"/>
</center>

#### Kardinalität (= Multiplizität)

Definiert die Anzahl der Instanzen, die unter diesem Attribut abgelegt werden können.

<center>
<img src="images/VL08/Kardinalitaet.png" alt="Kardinalitaet" width="600"/>
</center>

<center>
<img src="images/VL08/Kard_Uebers.png" alt="Kard_Uebers" width="600"/>
</center>


##### Kardinalität
* Anzahl der Objekte in einer Beziehung

##### Assoziationsname
* Optionaler Name der Assoziation

##### Rolle
* Definition der Verwendung einer Klasse
* Beispiel:
    * Ein Dozent ist ein Lehrer und ein Seminar wird als Vorlesung abgehalten
* Kardinalität sagt:
    * Ein Dozent kann 0 oder mehr Seminare als Form einer Vorlesung halten
    * Ein Seminar wird von einem oder mehr Dozenten gehalten werden

#### Rollenname

<center>
<img src="images/VL08/Rollenname.png" alt="Rollenname" width="600"/>
</center>

#### Assoziationen mit xor-Einschränkung

<center>
<img src="images/VL08/xor.png" alt="xor" width="600"/>
</center>

#### Assoziationsklassen

<center>
<img src="images/VL08/Assoziationsklassen.png" alt="Assoziationsklassen" width="600"/>
</center>

#### Aggregation
* eine Aggregation stellt eine schwache Beziehung zwischen dem "Ganzen" und einem "Teil" dar
* die Navigierbarkeit geht nur in die Richtug "Ganz" -> "Teil"
* keine Einschränkung der Multiplizität
    * Angabe der Multiplizität ist beliebig möglich
    * ein "Teil" kann in mehreren "Ganzen" vorhanden sein
    * bei keiner Angabe der Multiplizität wird sie auf "1" gesetzt

<center>
<img src="images/VL08/bsp_aggr.png" alt="bsp_aggr" width="600"/>
</center>

* In dem Beispiel hat ein Auto einen Motor, der Motor kann aber ausgetauscht werden. Das Auto wird als "Ganzes" gesehen, der Motor als "Teil", kann aber ohne das Ganze existieren

#### Komposition
* eine Komposition stellt eine starke Beziehung zwischen einem "Ganzen" und einem "Teil" dar
    * diese Assoziation ist "untrennbar"
* bei der Zerstörung des Ganzen, wird das Teil auch zerstört
    * das Zeil kann ohne dem Ganzen nicht existieren
* die Navigierbarkeit geht nur in die Richtung "Ganz" -> "Teil"
* die Multiplizität ist beschränkt
    * ein Ganzes kann belibig viele Teile haben
    * ein Teil kann zur zu einem Ganzen gehören
    * die Erlaubten Multiplizitäten sind 0, 0..1, 1
    * bei keiner Angabe wird die Multiplizität auf 1 gesetzt

<center>
<img src="images/VL08/bsp_komp.png" alt="bsp_komp" width="300"/>
<img src="images/VL08/bsp2_komp.png" alt="bsp2_komp" width="300"/>
</center>

#### Zusammenfassende Tabelle für UML-Klassendiagramme
<center>
<img src="images/VL08/uml_tabelle.png" alt="uml_tabelle" width="600"/>
</center>

### Logisch-statische Sicht auf ein Softwaresystem mit Analyseklassendiagrammen in der Systemanalyse

### Best Practices

### Beispiel