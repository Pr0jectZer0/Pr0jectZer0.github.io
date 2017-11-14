Vorlesung 4: Agile Workflows und Tools
-------------


**Inhalt:** Was bedeutet Continuous Integration, Continuous Delivery und Continuous Deployment und wie unterscheiden Sie sich? Was sind Build-Server und wofür werden Sie benötigt?

----------

**Continuous Integration:** 
ist eine Praxis in der Softwareentwicklung. Dabei werden isolierte Änderungen sofort geprüft und zur Gesamtcodebasis einer Software hinzugefügt.

> **Um dies zu erreichen, umfasst Continuous Integration folgendes:**

> - Entwickler führen mindestens einmal am Tag einen Check-In ihres Codes durch
> - Der Code wird bei jedem Check-In gebaut
> - Code wird bei jedem Check-In automatisch mit Unit-Tests getestet
> - Jeder hat Zugriff auf den Build und die Testreports
> - Der Build ist schnell, sodass Entwickler schnell Feedback bekommen
> - Tests werden in einer herunterskalierten Version der Produktionsumgebung ausgeführt

Wird kontinuierliche Integration richtig angewandt, bietet der Ansatz verschiedene **Vorteile**, wie z.B. ständige Feedbacks zum Status der Software. Zudem können Mängel bereits in einem frühen Entwicklungsstadium erkannt werden, sodass zukünftige Softwarefehler kleiner sowie weniger komplex ausfallen und sich somit einfacher beseitigen lassen. 

**Ziel** der kontinuierlichen Integration ist es, ein unmittelbares Feedback bieten zu können, so dass ein versehentlich integrierter Fehler so schnell wie möglich identifiziert und korrigiert wird. 

Wenn diese Bedingungen umgesetzt werden, ist man auf einem „reifen“ CI-Level und bereit für den nächsten Schritt: **Continuous Delivery**.

----------

**Continuous Delivery:** 
bezeichnet in der Softwareentwicklung eine Sammlung von Techniken, Prozessen und Werkzeugen, welche kurze Entwicklungszyklen mit häufigen Softwareupdates bis hin zum produktiven System ermöglicht. Dies wird ermöglicht durch eine weitgehend automatisierte „Deployment pipeline“ bzw. „Delivery pipeline“ mit automatisierten Build-Prozessen, Auslieferungen, Installationen, Tests (Continous Integration) und Deployments. 

Die **Vorteile** dieses Vorgehens sind zum einen geringere Kosten wegen höherer Automatisierung und höhere Zuverlässigkeit durch mehr automatisierte Tests sowie schnelleres Entdecken von Fehlern.

**Ziel:** Mit jeder erfolgreich durchlaufenden Umgebung wächst die Wahrscheinlichkeit, dass die Software auch in der Produktiv-Umgebung lauffähig sein wird. Ziel ist es somit, den Schritt in die Produktion soweit vorzubereiten, dass im Prinzip „per Knopfdruck“ in die Produktion gegangen werden kann.

----------

Der letzte Schritt ist **Continous Deployment**. Beim Continous Delivery legt man fest, wann man in Produktion geht, beim Continous Deploment hingegen ist es keine Wahl die sich manuell steuern lässt, sondern ein automatisierter Prozess.

Die **Vorteile** sind ein noch schnelleres Feedback, da jede Änderung direkt in Produktion geht und somit das Zeitfenster für eine verlorene Gelegenheit sehr klein ist. 

----------

**Build-Server:**
stellen einen zentralen Ort dar, an dem der aktuelle Stand der Software (in Form von Testergebnissen und kompilierten Artefakten) einsehbar ist. Build-Server werden üblicherweise als Continuous Integration Server oder einfach CI-Server bezeichnet, wobei alle Prozesse innerhalb eines Build-Server vollautomatisch ablaufen und somit Fehler durch falsche, ausgelassene oder vertauschte Prozess-Schritte ausgeschlossen werden. Über die kontinuierliche Integration hinaus können Build-Server Continuous Deployment ermöglichen und Updates für die Produktion bereitstellen, wenn Builds erfolgreich sind und alle Tests bestehen. 
**Beispiele** für einen Build-Server sind z.B. Jenkins und Travis CI.

----------

>**Quellenverzeichnis:**

> - Informationen zu Continuous Integration [hier][1]
> - Informationen zu Continuous Delivery [hier][2]
> - Informationen zu Continous Deployment [hier][3]
> - Unterschiede dieser Workflows [hier][4]
> - Informationen zu Build-Server [hier][5]


  [1]: http://www.searchenterprisesoftware.de/definition/Kontinuierliche-Integration-Continuous-Integration
  [2]: http://www.torsten-horn.de/techdocs/ContinuousDelivery.html
  [3]: https://de.wikipedia.org/wiki/Continuous_Delivery
  [4]: https://www.scrum.de/unterschiede-zwischen-continuous-integration-continuous-delivery-und-continuous-deployment/
  [5]: http://deviq.com/build-server/
