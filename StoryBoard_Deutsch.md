# OER zu Geospatial Web Services (in Arbeit!)       
         	           	
## 1. Überblick

In dieser Open Educational Resource (OER) lernst du, welche Formen von **Geospatial Web Services** existieren, wie sie strukturiert sind, wie sie in ein Open Source GIS (QGIS) integriert und über GeoServer veröffentlicht werden können. 

**Nachdem du die folgende OER abgeschlossen hast, wirst du wissen:**
* was Geospatial Web Services und OGC-Standards sind
* wo Sie nützliche Geospatial Web Services finden und identifizieren können und wie sie strukturiert sind
* wie man Web Services in QGIS integriert und mit Daten daraus arbeitet 
* wie man seine eigenen Web Services mit GeoServer veröffentlicht 

**Das OER ist wie folgt aufgebaut**

1. Überblick
2. Thematischer Hintergrund 
3. Übungen und Leitfäden
4. Quiz 
5. Zusammenfassung 

**Generelle Informationen**

Dieses Tutorial richtet sich hauptsächlich an Teilnehmer, die in etwa ... Minuten ihre Fähigkeiten zur Integration von Daten aus Geospatial Web Services verbessern wollen. Du solltest bestenfalls einige Grundkenntnisse im Umgang mit GIS-Software besitzen.

Dieses Tutorial wurde am Institut für Geodäsie der Fachhochschule Bochum in enger Zusammenarbeit mit der Universität Münster und der Universität Bochum entwickelt. Hauptautor ist Fabian Przybylak unter der Leitung von Prof. Dr. Carsten Keßler.

Du darfst das OER (H5P-Inhalte) unter den Bedingungen der CC-BY-SA 4.0-Lizenz frei verwenden, verändern und vervielfältigen. Jeglicher Code, der mit dem OER zur Verfügung gestellt wird, kann unter den Bedingungen der MIT-Lizenz verwendet werden. Bitte lesen Sie die [vollständigen Lizenzbedingungen](/LICENSE.md). 

Das Projekt OER4SDI wurde von der Digitalen Hochschule NRW empfohlen und wird durch das Ministerium für Kultur und Wissenschaft NRW gefördert. 

## 2. Thematischer Hintergrund

**Gliederung des thematischen Hintergrunds** 
* Kurze Einleitung mit allgemeinem Kontext und Hintergrund (in wenigen Sätzen) 
* Inhaltliche Vertiefung (Videoformat + Textakkordion welches die gegebenen Informationen zusammenfasst)


### 2.1 Kurze Einführung

**Worum geht es eigentlich?**
Die rasche Entwicklung von Methoden und Techniken zur Erfassung von Geodaten bietet die Möglichkeit, riesige Mengen von Geodaten zu sammeln. Sie stellt jedoch auch verschiedene Datenorganisationen und Datennutzer vor die Herausforderung, große Mengen von Geodaten zu verwalten, gemeinsam zu nutzen, zu verarbeiten und zu analysieren. Datenorganisationen stehen vor der Herausforderung, neue Lösungen für die Verwaltung, Speicherung und gemeinsame Archivierung dieser riesigen Datenmengen zu finden.

Ein Online-Dienst um geografische Informationen und räumliche Daten über das Internet bereit zu stellen sind Geospatial Web Services. Diese Dienste ermöglichen es Benutzern, geografische Daten effizient zu teilen, zu suchen, zu visualisieren, abzurufen und zu analysieren.

**Welches Problem besteht dabei?**
Datenverbreitungssysteme müssen sich immer mit einem Heterogenitätsproblem auseinandersetzen. Verschiedene Quellen können die Effektivität des Austauschs und der Verwaltung von Geodaten behindern. Verschiedene Betriebssysteme, Hardware, Software, Datenformate und Schnittstellen sind mit dem Problem der syntaktischen Heterogenität verbunden. Wenn zwei Webdienste die Schnittstellen des jeweils anderen nicht kennen, können sie keine Nachrichten und Daten austauschen.

**Welche Lösung gibt es dafür?**
Aus diesem Grund sind Geospatial Web Services in der Regel nach den vom Open Geospatial Consortium entwickelten OGC-Standards organisiert. Diese Standards ermöglichen, dass die Services interoperabel sind und von verschiedenen Anwendungen und Plattformen übergreifend verwendet werden können.

### 2.2 Inhaltliche Vertiefung (Video)

**Was sind Geospatial Webdienste?**
Geospatial Web Services sind eine Art von Webdiensten, die es ermöglichen, Geodaten und -dienste im Internet bereitzustellen, abzurufen und zu verarbeiten. Diese Dienste werden in der Regel von Geodaten- oder GIS-Organisationen, Regierungsbehörden, Unternehmen und anderen Einrichtungen bereitgestellt, die Geodaten verwalten.
![](Single_Learning_Element/Img/Slide1.png) 
**Wofür braucht man Geospatial Web Services?**
Durch die Verwendung von Geospatial Web Services können Benutzer auf Geodaten von verschiedenen Quellen zugreifen, umfassende Analysen durchführen und maßgeschneiderte Anwendungen und Visualisierungen erstellen.

**Wie sind GWS aufgebaut und gibt es vorherrschende Standards?**
Geospatial Web Services sind strukturiert, um geografische Daten und Funktionalitäten über das Web bereitzustellen. Sie basieren in der Regel auf einer Client-Server-Architektur, bei der der Client (in der Regel ein Webbrowser) eine Anfrage an den Server stellt und dieser daraufhin geografische Daten und Funktionalitäten zurückliefert.

Geospatial Web Services verwenden in der Regel eine oder mehrere standardisierte Schnittstellen, die von dem Open Geospatial Consortium (OGC) spezifiziert wurden. Die OGC-Schnittstellen definieren das Format und die Struktur der Daten, die vom Server zurückgegeben werden, sowie die Methoden und Parameter, mit denen die Daten abgefragt werden können.
![](Single_Learning_Element/Img/Slide2.png) 
**Was ist das OGC?**
Das OGC oder auch Open Geospatial Consortium ist eine gemeinnützige Organisation, die sich auf die Entwicklung von Standards für Geodaten und Geodienste konzentriert. Die Organisation wurde im Jahr 1994 gegründet und hat ihren Hauptsitz in den USA.

Das Ziel des OGC ist es, offene Standards für Geodaten und -dienste zu entwickeln und zu fördern, um die Interoperabilität und den Austausch von Geodaten und -diensten zwischen verschiedenen Systemen, Anwendungen und Organisationen zu erleichtern. Die OGC-Standards umfassen Protokolle für den Zugriff auf Geodaten (z.B. WMS, WFS, WCS), Datenmodellierung, Geoprocessing, Metadaten, Katalogisierung und vieles mehr.

Das OGC Consortium arbeitet eng mit anderen Standardisierungsorganisationen und Regierungsbehörden weltweit zusammen, um sicherzustellen, dass die Standards für Geodaten und -dienste in verschiedenen Anwendungsbereichen und in verschiedenen Ländern harmonisiert sind.

Die Mitgliedschaft im OGC steht Organisationen und Einzelpersonen aus der Geodaten- und Geodienstbranche offen und bietet ihnen die Möglichkeit, an der Entwicklung von Standards teilzunehmen und von der Zusammenarbeit mit anderen Fachleuten zu profitieren.
![](Single_Learning_Element/Img/Slide3.png) 
**Wie sehen die OGC-Architekturelemente und die wichtigsten OGC-Standards aus?**
Die OGC Web Services-Architektur besteht aus einer Reihe von Komponenten, die zusammenarbeiten, um die verschiedenen Arten von Geodaten-Webdiensten bereitzustellen. Die wichtigsten Komponenten sind:

* **Service Provider:** Dies ist der Server, der den Webdienst bereitstellt und auf Anfragen von Clients antwortet.
* **Service Requester:** Dies ist der Client, der den Webdienst anfordert und auf die Antwort vom Service Provider wartet.
* **Service Registry:** Dies ist ein Verzeichnis, das Informationen über verfügbare Geodaten-Webdienste enthält, damit Service Requester diese finden und verwenden können.
* **Service Broker:** Dies ist ein Vermittler, der die Interoperabilität zwischen verschiedenen Geodaten-Webdiensten ermöglicht, indem er Daten und Anfragen zwischen ihnen übersetzt.
![](Single_Learning_Element/Img/Slide4.png) 
Geospatial Web Services verwenden offene Standards und Protokolle, um den Austausch von Geodaten zwischen verschiedenen Systemen und Plattformen zu erleichtern. Zu den wichtigsten Standards gehören: 

* Web Map Service (**WMS**) 
* Web Feature Service (**WFS**)
* Web Coverage Service (**WCS**)
* Catalog Service (**CSW**)
* Sensor Observation Service (**SOS**)

**Was ist der Unterschied zwischen den verschiedenen Services?**
* Ein Web Map Service (**WMS**) ermöglicht es einem Client, statische Kartenbilder von einem Server abzurufen und anzuzeigen.
* Ein Web Feature Service (**WFS**) ermöglicht den Zugriff auf und die Abfrage von vektorbasierten Geodaten.
* Ein Web Coverage Service (**WCS**) ermöglicht den Zugriff auf und die Abfrage von räumlichen Rasterdaten wie Satellitenbildern oder Höhenmodellen.
* Ein Catalog Service (**CSW**) ermöglicht es einem Client, Metadaten über verfügbare Geodaten und -dienste zu suchen und abzurufen.
* Ein Sensor Observation Service (**SOS**) ermöglicht den Zugriff auf Echtzeitdaten von Sensoren, z.B. Umweltsensoren.
![](Single_Learning_Element/Img/Slide5.png) 
**Wie sieht eine typische Web-Anfrage für einen Web map Service aus?**
Das Web Map Service (WMS) Protokoll ist eine von dem Open Geospatial Consortium (OGC) definierte Schnittstelle, die es ermöglicht, Karten und geografische Daten über das Web abzufragen und zu visualisieren. Das WMS-Protokoll definiert das Format und die Struktur der Daten, die vom Server zurückgegeben werden, sowie die Methoden und Parameter, mit denen die Daten abgefragt werden können.

Das WMS-Protokoll verwendet HTTP oder HTTPS als Transportprotokoll. Eine typische WMS-Anfrage besteht aus einer URL, die verschiedene Parameter enthält, die den Inhalt der Karte bestimmen. Hier ist ein Beispiel einer WMS-Anfrage und der zugehörigen Parameter:
![](Single_Learning_Element/Img/Slide6.png) 
Der Server verarbeitet die Anfrage und sendet die Karte als Antwort im angeforderten Format zurück. Die Karte kann dann im Browser oder in einer Anwendung angezeigt werden.

**Welche weiteren Anfragen können an einen WMS-Server gestellt werden?**
Ein WMS-Protokoll definiert noch weitere Anfragen, die von einem Client an einen WMS-Server gesendet werden können.

* **GetCapabilities:** Mit dieser Anfrage kann der Client Informationen über die verfügbaren Layer und Funktionen des WMS-Servers abrufen. Die Antwort enthält eine XML-Datei, die die verfügbaren Layer, ihre Eigenschaften und Metadaten sowie die unterstützten Operationen und Formate enthält.
* **GetMap:** Mit dieser Anfrage kann der Client eine Karte vom Server abrufen. Die Parameter dieser Anfrage umfassen den gewünschten Ausschnitt der Karte, die Größe und das Format der Karte sowie die gewünschten Layer und Stile.
* **GetFeatureInfo:** Mit dieser Anfrage kann der Client Informationen über die Eigenschaften von Objekten in einem bestimmten Punkt auf der Karte abrufen. Die Antwort enthält eine XML-Datei oder ein anderes Format, das die Attribute und Werte der Objekte enthält.
* **DescribeLayer:** Mit dieser Anfrage kann der Client Informationen über die Eigenschaften und Metadaten eines bestimmten Layers abrufen. Die Antwort enthält eine XML-Datei oder ein anderes Format, das die Eigenschaften und Metadaten des Layers enthält.

Es gibt auch andere Anfragen wie **GetLegendGraphic** und **GetStyles**, die für bestimmte Anwendungsfälle nützlich sein können.
![](Single_Learning_Element/Img/Slide7.png) 
**Welche weiteren Anfragen können an einen WFS-Server gestellt werden?**
Ein Web Feature Service (WFS) Server verwendet andere Anfragen als ein Web Map Service (WMS) Server, da der WFS-Standard sich auf den Zugriff und die Abfrage von vektorbasierten Geodaten konzentriert, während der WMS-Standard die Visualisierung von Karten im Fokus hat.

* **GetCapabilities:** Mit dieser Anfrage kann der Client Informationen über die verfügbaren Layer und Funktionen des WFS-Servers abrufen. Die Antwort enthält eine XML-Datei, die die verfügbaren Layer, ihre Eigenschaften und Metadaten sowie die unterstützten Operationen und Formate enthält.
* **DescribeFeatureType:** Mit dieser Anfrage kann der Client die Struktur eines bestimmten Layers abrufen. Die Antwort enthält eine XML-Datei, die die Eigenschaften und Attribute des Layers definiert.
* **GetFeature:** Mit dieser Anfrage kann der Client vektorbasierte Geodaten aus einem oder mehreren Layern abrufen. Die Parameter dieser Anfrage umfassen den gewünschten Ausschnitt der Daten, die Attribute und Eigenschaften, die zurückgegeben werden sollen, und die Filterbedingungen, die auf die Daten angewendet werden sollen.
* **Transaction:** Mit dieser Anfrage kann der Client Änderungen an den Daten auf dem WFS-Server vornehmen. Die Operationen können Insert, Update oder Delete sein, und sie werden in einer XML-Datei definiert, die an den Server gesendet wird.

Es gibt ebenfalls noch andere Anfragen wie **LockFeature**, **GetPropertyValue** und **GetFeatureWithLock**.
![](Single_Learning_Element/Img/Slide8.png) 
**Was ist GeoServer?**
GeoServer wurde erstmals im Jahr 2001 von der Open Source Geospatial Foundation (OSGeo) ins Leben gerufen. Die Idee hinter GeoServer war, eine Open-Source-Software zu schaffen, die es Benutzern ermöglicht, Geodaten im Web zu verwalten und bereitzustellen.

Die ursprüngliche Version von GeoServer wurde von der australischen Regierungsbehörde Geoscience Australia entwickelt und als Open-Source-Software veröffentlicht. Im Laufe der Jahre wurde GeoServer von einer breiten Community von Entwicklern weiterentwickelt und verbessert, die neue Funktionen hinzufügten und die Leistung und Stabilität der Software verbesserten.

GeoServer hat seit seiner Gründung eine starke Unterstützung von der OSGeo-Community erfahren. Die OSGeo ist eine gemeinnützige Organisation, die sich der Förderung von Open-Source-Geodaten-Software widmet und GeoServer ist eines ihrer wichtigsten Projekte. GeoServer hat auch eine aktive Benutzer-Community und wird von vielen Regierungsbehörden, Unternehmen und gemeinnützigen Organisationen auf der ganzen Welt eingesetzt.

Heute ist GeoServer eine der beliebtesten Open-Source-Softwarelösungen für Geodatenmanagement und -bereitstellung im Web. Es ist bekannt für seine Flexibilität, Skalierbarkeit und Leistung und wird von einer wachsenden Anzahl von Entwicklern und Benutzern weltweit genutzt.
![](Single_Learning_Element/Img/Slide9.png) 
**Welche Funktionen hat GeoServer?**
GeoServer bietet eine Plattform für die Verwaltung und Veröffentlichung von Geodaten im Web, indem es Daten in verschiedenen Geodatenformaten (wie zum Beispiel Shapefiles, Geotiffs, PostGIS-Datenbanken) verarbeitet und sie als Webdienste (wie zum Beispiel WMS, WFS, WCS) bereitstellt.

Die Funktionen von GeoServer umfassen:

* **Datenmanagement:** GeoServer ermöglicht es Benutzern, Geodaten aus verschiedenen Quellen zu importieren und zu verwalten. Es unterstützt verschiedene Datenformate, einschließlich Vektor- und Rasterdaten, sowie Datenbanken wie PostGIS, Oracle und MySQL.
* **Datenverarbeitung:** GeoServer kann Daten transformieren und filtern, um sie in verschiedenen Formaten und Projektionen bereitzustellen. Es kann auch Daten aggregieren und Gruppierungen erstellen, um benutzerdefinierte Ansichten bereitzustellen.
* **Bereitstellung von Webdiensten:** GeoServer bietet eine breite Palette von Webdiensten, einschließlich Web Map Service (WMS), Web Feature Service (WFS) und Web Coverage Service (WCS). Diese Webdienste ermöglichen es Benutzern, Geodaten auf einfache Weise über das Internet zu visualisieren, zu analysieren und herunterzuladen.
* **Sicherheit:** GeoServer bietet eine robuste Sicherheitsinfrastruktur, die es Benutzern ermöglicht, den Zugriff auf Geodaten zu steuern. Es unterstützt Authentifizierung und Autorisierung, sowie HTTPS-Verschlüsselung für sichere Datenübertragung.
* **Skalierbarkeit:** GeoServer kann auf einer Vielzahl von Plattformen ausgeführt werden, einschließlich Desktop-Computern, Servern und Cloud-Infrastrukturen. Es ist auch in der Lage, hohe Lasten zu bewältigen und bietet eine hohe Verfügbarkeit und Leistung.

Insgesamt ist GeoServer eine leistungsstarke und vielseitige Plattform für die Verwaltung und Bereitstellung von Geodaten im Web. Die es Benutzern ermöglicht, Geodaten auf einfache Weise zu verwalten und zu teilen, was es zu einem wichtigen Werkzeug für Geodateninfrastrukturen macht.
![](Single_Learning_Element/Img/Slide10.png) 
## 3. Übungen und Leitfäden

**Aufbau der Übungen und Leitfäden** 
* Aufgabenstellung 
* Videoguide (Screencast)

### 3.1 Übung 1

**Benötigte Softwarekomponenten, die in dieser Übung verwendet werden:** 

**QGIS** ist eine freie und quelloffene, plattformübergreifende Desktop-Anwendung für geografische Informationssysteme (GIS), die das Anzeigen, Bearbeiten, Drucken und Analysieren von Geodaten unterstützt. 
(Sie können **QGIS** über die [offizielle Webseite](https://qgis.org/de/site/forusers/download.html) installieren und der dortigen Anleitung folgen)

**Aufgabenstellung**

Stöbere einige Zeit auf den Webseiten der angehängten Linksammlung und prüfe welche Services auf den Webseiten angeboten werden. Achte zusätzlich darauf in welcher Form die Services bereitstehen (WMS, WFS, etc.).

* [Geodatenkatalog Deutschland](https://gdk.gdi-de.org/gdi-de/srv/ger/catalog.search#/home)
* [Geoportal Deutschland](https://www.geoportal.de/) 
* [Geodatenkatalog Schweiz](https://www.geocat.ch/geonetwork/srv/ger/catalog.search#/home)

Du hast nun einige Quellen kennengelernt über die du Geospatial Web Services finden kannst. Wähle im folgenden einen WMS- und einen dazu passenden WFS-Service aus und implementiere diese in ein simples QGIS Projekt. Folge dazu gerne auch dem angehängten Videoguide. 

Falls ein Service mal nicht funktionieren sollte dann probiere zunächst einen anderen aus. Es kann vorkommen, dass Services vom Provider nicht mehr unterstützt werden oder Links nicht mehr aktuell sind. 

**Inhalt des Videoguides**

Das Skript zum Videoguide findest du [hier](https://github.com/oer4sdi/Geospatial-Web-Services/blob/main/Single_Learning_Element/Text/Skript%20Videoguide%201%20Modul%201.docx) 

Das Vollständige Video findest du [hier](https://github.com/oer4sdi/Geospatial-Web-Services/tree/main/Single_Learning_Element/Video) 

### 3.2 Übung 2
**Benötigte Softwarekomponenten, die in dieser Übung verwendet werden:** 

**QGIS** ist eine freie und quelloffene, plattformübergreifende Desktop-Anwendung für geografische Informationssysteme (GIS), die das Anzeigen, Bearbeiten, Drucken und Analysieren von Geodaten unterstützt.

**GeoServer** ist ein in Java geschriebener Open-Source-Server, der es Benutzern ermöglicht, Geodaten gemeinsam zu nutzen, zu verarbeiten und zu bearbeiten.

**Aufgabenstellung**

Lade dir die zur Verfügung gestellten Geodaten herunter und schaue dir das Folgende Video an. Deine Aufgabe besteht darin dem Screencast zu Folgen und selbst einen WMS- und einen WFS-Service Local auf deinem System zu hosten. Prüfe anschließend in QGIS ob du erfolgreich warst,  indem du die Services in ein neues QGIS-Projekt einbindest. 

Falls du dich noch tiefer mit dem Thema beschäftigen willst, dann findest du weitere Tutorials in der [offiziellen Dokumentation](https://docs.geoserver.org/) von GeoServer. 

**Inhalt des Videoguides**

Das Skript zum Videoguide findest du [hier](https://github.com/oer4sdi/Geospatial-Web-Services/blob/main/Single_Learning_Element/Text/Skript%20Videoguide%202%20Modul%201.docx) 

Das Vollständige Video findest du [hier](https://github.com/oer4sdi/Geospatial-Web-Services/tree/main/Single_Learning_Element/Video) 

Installation von Geoserver über Docker


```shell
docker pull docker.osgeo.org/geoserver:2.22.0
```

Ausführen des Docker Images 

```shell
docker run -it -p 80:8080 docker.osgeo.org/geoserver:2.22.0
```

Check http://localhost/geoserver

## 5. Quiz


## 5. Zusammenfassung

Hey! Das hast du gut gemacht! Wir hoffen, dass Sie nun eine Vorstellung davon haben, wie Sie mit Geospatial Web Services wie WMS und WMF Services in Ihrem GIS arbeiten und wie Sie Ihre eigenen Web Services über Geoserver einrichten können.  


**Interessiert daran, mehr zu lernen?**

Im Internet finden Sie eine Fülle von Ressourcen zu Geospatial Web Services. Hier sind einige Empfehlungen: 

* [Zhao, P., & Di, L. (Eds.). (2010). Geospatial Web Services: Advances in information interoperability: Fortschritte bei der Interoperabilität von Informationen. IGI Global.](https://www.igi-global.com/book/geospatial-web-services/46010) 
* [Kralidis, A. T. (2007). Geospatial Web Services (Geodaten-Webdienste): The evolution of geospatial data infrastructure. In The Geospatial Web (S. 223-228). Springer, London.](https://link.springer.com/chapter/10.1007/978-1-84628-827-2_22) 
* [van den Brink, L., Barnaghi, P., Tandy, J., Atemezing, G., Atkinson, R., Cochrane, B., ... & Janowicz, K. (2019). Best Practices für die Veröffentlichung, Abfrage und Nutzung von Geodaten im Web. Semantic Web, 10(1), 95-114.](https://content.iospress.com/articles/semantic-web/sw305)
* [Clabby, J. (2003). Webdienste erklärt: Lösungen und Anwendungen für die reale Welt. Prentice Hall Professional.](https://books.google.be/books?hl=nl&lr=&id=AKkFqV9-_9AC&oi=fnd&pg=PR13&dq=%22fundamentals+of+web+services%22&ots=PL1iLMeHGW&sig=H9XAty66RX8LFIKAo9-VmOOEZDA#v=onepage&q=%22fundamentals%20of%20web%20services%22&f=false)
* [Link zu einer Seite oder einer Vorlesung, die OGC WMS in einer einfachen Sprache beschreibt](https://www.ogc.org/standards/wms/introduction) 
* [Link zu einer Seite oder einer Vorlesung, die OGC WFS in einfacher Sprache beschreibt](http://opengeospatial.github.io/e-learning/wfs/text/basic-main.html)
* [Link zu Geospatial Web Services](https://gis4schools.readthedocs.io/en/latest/part2/2_1.html)


**Ihr Feedback ist willkommen!**

Wenn Sie Defizite in diesem OER-Modul festgestellt haben oder Ideen zur Verbesserung des OER-Materials haben, sind Sie herzlich eingeladen, Einträge in die Issue-Liste im [Github repository dieses OERs](https://github.com/oer4sdi/Geospatial-Web-Services).
