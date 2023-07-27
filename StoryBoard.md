# OER zu Knowledge Graphen (in Arbeit!)       

In dieser Open Educational Resource (OER) lernst du, wie die Wissensmodellierung in Knowledge Graphen strukturiert ist, aus welchen Elementen sich die übergeordnete Vision des Semantic Webs zusammensetzt und mit welchen Techniken heutzutage praktische Anwendungsbeispiele von diesen Konzepten profitieren können. 

**Nachdem du das folgende OER abgeschlossen hast, wirst du wissen:**

* Was Knowledge Graphen, das Semantic Web und Linked Data sind
* Wie die übergeordnete Vision eines Semantic Web aussieht und in wie weit die Vision zur Realität geworden ist 
* Welche technischen Ansätze zur Umsetzung entwickelt wurden 
* Was es für praktische Anwendungsbeispiele im Kontext von Geodateninfrastrukturen gibt 
* Wie du selbst einfache Abfragen erstellen kannst und Ansätze des Semantic Web für dich nutzen kannst

**Das OER ist wie folgt aufgebaut**

1. Überblick
2. Thematischer Hintergrund 
3. Übungen und Leitfäden
4. Quiz 
5. Zusammenfassung 

**Generelle Informationen**

Dieses Tutorial richtet sich hauptsächlich an Teilnehmer, die in etwa 30 Minuten ihre Kenntnisse zu den Konzepten der Knowledge Graphen, dem Semantic Web und Linked Data verbessern wollen.

Dieses Tutorial wurde am Institut für Geodäsie der Fachhochschule Bochum in enger Zusammenarbeit mit der Universität Münster und der Universität Bochum entwickelt. Hauptautor ist Fabian Przybylak unter der Leitung von Prof. Dr. Carsten Keßler und in Zusammenarbeit mit Lucas Rudnik.

Du darfst das OER (H5P-Inhalte) unter den Bedingungen der CC-BY-SA 4.0-Lizenz frei verwenden, verändern und vervielfältigen. Jeglicher Code, der mit dem OER zur Verfügung gestellt wird, kann unter den Bedingungen der MIT-Lizenz verwendet werden. Bitte lesen Sie die [vollständigen Lizenzbedingungen](/LICENSE.md). 

Das Projekt OER4SDI wurde von der Digitalen Hochschule NRW empfohlen und wird durch das Ministerium für Kultur und Wissenschaft NRW gefördert.

## 2. Thematischer Hintergrund

**Gliederung des thematischen Hintergrunds**
* Kurze Einleitung mit allgemeinem Kontext und Hintergrund (in wenigen Sätzen) 
* Inhaltliche Vertiefung (Texte welche die gegebenen Informationen zusammenfasst + Videoformat)


### 2.1 Kurze Einführung

**Die Geschichte des Semantic Web, der Knowledge Graphen und des Linked Data Konzepts**

Eine syntaktische Interoperabilität bezieht sich auf den korrekten Austausch von Daten, basierend auf gemeinsamen Standards für die Datenstruktur und das Format. Eine semantische Interoperabilität hingegen betrifft das einheitliche Verständnis und die Interpretation der Bedeutung und des Kontexts der Daten. Während die syntaktische Interoperabilität sicherstellt, dass Daten fehlerfrei übertragen werden, ermöglicht die semantische Interoperabilität ein gemeinsames Verständnis der Dateninhalte und deren korrekte Interpretation im entsprechenden Kontext. Beide Aspekte sind wichtig, um effektive Kooperation und Kommunikation zwischen verschiedenen Systemen zu gewährleisten.

Ein Semantisches Web ist mittlerweile keine neue Idee mehr, aber die Vision hat nichts von ihrer Aktualität verloren. Um die aktuellen Entwicklungen zu verstehen, kann ein Blick zurück zu den Anfängen sehr aufschlussreich sein:

![](Single_Learning_Element/Img/Zeitstrahl/Zeitstrahl.png)

### 2.2 Inhaltliche Vertiefung - Konzepte und Vision(Video)

**Die Vision eines Semantic Webs**

Das Semantic Web ist ein Konzept, dass von Tim Berners-Lee, dem Erfinder des World Wide Web, geprägt wurde. Es handelt sich dabei um eine Erweiterung des klassischen Web, die darauf abzielt, die Maschinenlesbarkeit von Informationen im Web zu verbessern und somit die Effizienz und die Qualität der Webanwendungen zu steigern.

Das klassische Web ist eine unerschöpfliche Quelle von Informationen, aber die meisten Informationen sind unstrukturiert und nur für menschliche Leser verständlich. Im Gegensatz zum klassischen Web, in dem Informationen von Menschen gelesen werden, sollen Maschinen durch das Semantic Web in der Lage sein, Informationen automatisch zu verarbeiten und zu verstehen. Dadurch können neue Anwendungen und Dienste entwickelt werden, die auf intelligentere Weise mit den Informationen im Web umgehen.

**Die Integration des Linked Data Konzepts**

Linked Data ist ein Konzept, dass auf dem Semantic Web aufbaut. Es bezieht sich auf die Verknüpfung von Daten, die auf verschiedenen Webseiten und in verschiedenen Datenbanken gespeichert sind. Dadurch können Daten automatisch verknüpft und abgefragt werden, ohne dass der Benutzer die genaue Speicherposition oder Datenstruktur kennen muss. Linked Data spielt eine wichtige Rolle im Semantic Web, da es dazu beiträgt, die Vernetzung von Informationen zu fördern und somit das Potenzial des Semantic Web voll auszuschöpfen.

**Die Entwicklung von Knowledge Graphen**

Ein Knowledge Graph ist eine strukturierte Datenbank, die Informationen über Entitäten und deren Beziehungen enthält. Wissen wird in Form von Graphen dargestellt, wobei Knoten Entitäten und Kanten Beziehungen zwischen den Entitäten repräsentieren.

Im Gegensatz zu herkömmlichen Datenbanken, die oft tabellarisch organisiert sind, ermöglicht ein Knowledge Graph eine flexible Darstellung von Wissen und kann semantische Zusammenhänge zwischen verschiedenen Entitäten erfassen. Die Funktionsweise basiert auf dem Konzept des semantischen Webs und oft wird das Resource Description Framework (RDF) als Datenmodell genutzt.

Ein Knowledge Graph kann Informationen aus verschiedenen Quellen wie strukturierten Datenbanken, unstrukturierten Texten, Webseiten, APIs usw. zusammenführen. Dies erlaubt es, Wissen in einer maschinenlesbaren Form zu speichern und ermöglicht so die Verknüpfung und Abfrage von Informationen auf einer tieferen semantischen Ebene.

Knowledge Graphen werden in verschiedenen Bereichen eingesetzt, wie zum Beispiel in der Wissensorganisation, der semantischen Suche, der Datenintegration, dem maschinellen Lernen und der künstlichen Intelligenz. Sie bieten eine Grundlage für die Entwicklung von intelligenten Systemen, die Wissen verstehen, analysieren und daraus Schlussfolgerungen ziehen können.

### 2.3 Inhaltliche Vertiefung - Technische Umsetzung (Video)

Um Ansätze der technischen Umsetzung verstehen zu können müssen einige Schlüsseltechnologien und Begriffe erläutert werden.

**Kurz erklärt: Uniform Resource Identifier (URI)**

Uniform Resource Identifier (URI) sind Zeichenketten, die verwendet werden, um Ressourcen im World Wide Web eindeutig zu identifizieren. Eine URI dient als globaler Bezeichner für eine Ressource, sei es eine Webseite, eine Datei, ein Bild oder eine andere Art von digitaler Information.

URIs bestehen aus zwei Hauptkomponenten: dem Schema und dem spezifischen Identifikator. Das Schema gibt an, wie der Identifikator zu interpretieren ist, und kann beispielsweise "http://" für eine Webseite oder "file://" für eine lokale Datei sein. Der spezifische Identifikator ist der Teil, der die genaue Adresse oder den Pfad zur Ressource angibt.

Es gibt verschiedene Arten von URIs. Die bekannteste Form ist die Uniform Resource Locator (URL), die normalerweise verwendet wird, um Webseiten zu adressieren.<br>
<span style="color:red">*Eine URL enthält das Schema (z. B. "http://"), gefolgt von der Domain (z. B. "www.example.com") und dem Pfad zur spezifischen Ressource (z. B. "/pfad/zur/datei.html").*</span>

Ein weiterer Typ ist der Uniform Resource Name (URN), der dazu dient, Ressourcen unabhängig von ihrem aktuellen Speicherort dauerhaft und eindeutig zu identifizieren. URNs können verwendet werden, um zum Beispiel auf bibliografische Informationen, Dokumente oder andere digitale Objekte zu verweisen.

URIs spielen eine zentrale Rolle im Web, da sie die Grundlage für das Adressieren und Verlinken von Ressourcen bilden. Durch die Verwendung von URIs können Benutzer und Maschinen auf die gewünschten Ressourcen zugreifen, sei es durch das Eingeben der URI in einen Webbrowser oder durch das Klicken auf Hyperlinks, die auf URIs verweisen.

Es ist wichtig anzumerken, dass URLs und URNs eng miteinander verwandt sind und beide als Untergruppe von URIs betrachtet werden können. URLs dienen jedoch hauptsächlich dazu, Ressourcen zu lokalisieren, während URNs auf ihre Identität abzielen.

**Kurz erklärt: Resource Desciption Framework**

RDF (Resource Description Framework) ist ein Datenmodell des Semantic Web, das verwendet wird, um strukturierte Informationen über Ressourcen im Web zu beschreiben und zu verlinken.

Das RDF-Modell besteht aus drei grundlegenden Komponenten: Ressourcen, Eigenschaften und Werten. Eine Ressource wird durch eine URI (Uniform Resource Identifier) identifiziert und repräsentiert eine Entität im Web wie z.B. eine Person, ein Ort oder ein Dokument. Eine Eigenschaft (auch Prädikat genannt) beschreibt eine Beziehung zwischen zwei Ressourcen und wird ebenfalls durch eine URI identifiziert. Ein Wert gibt an, welcher Wert die Eigenschaft für die Ressource hat, die sie beschreibt.

RDF-Daten werden in Tripeln ausgedrückt, die aus einem Subjekt, einem Prädikat und einem Objekt bestehen. Das Subjekt ist die Ressource, auf die sich das Tripel bezieht, das Prädikat beschreibt die Beziehung zwischen dem Subjekt und dem Objekt, und das Objekt ist der Wert, der die Beziehung beschreibt. Die Tripel werden auch als "Sätze" oder "Statements" bezeichnet.

Ein Beispiel für ein RDF-Tripel könnte lauten: *"Tim" besitzt das Attribut " hat Alter" mit dem Wert "30". In diesem Fall ist "Tim" das Subjekt, "hat Alter" das Prädikat und "30" das Objekt.*

RDF ermöglicht es, komplexe Beziehungen zwischen Ressourcen im Web auszudrücken und zu verknüpfen, wodurch das Web zu einem globalen Wissensraum wird.
![](Single_Learning_Element/Img/RDF/RDF.png)
**Kurz erklärt: Web Ontology Language (OWL)**

OWL ist eine formale Sprache des Semantic Webs, die verwendet wird, um komplexe Ontologien zu definieren, also hierarchische und semantische Strukturen, die Wissen und Beziehungen zwischen Konzepten repräsentieren. Außerdem definiert OWL diese Beziehungen in einer maschinenlesbaren Form, die von Computerprogrammen verarbeitet werden kann.

OWL ist eine logische Sprache und basiert auf Beschreibungslogiken wie der Description Logic (DL). Diese Logik stellt verschiedene Konstruktoren zur Verfügung, um Ontologien zu modellieren, wie Klassen, Eigenschaften, Individuen, Einschränkungen, Abhängigkeiten, etc.

*Beispielsweise könnte eine Ontologie in OWL eine Hierarchie von Klassen definieren, z.B. "Tier" als übergeordnete Klasse von "Säugetier", "Vogel" und "Reptil". Darüber hinaus können Eigenschaften definiert werden, wie z.B. "hat Gewicht" oder "isst". Einschränkungen können auch definiert werden, um Beziehungen zwischen Klassen oder Eigenschaften zu beschreiben.*

OWL wird von vielen Werkzeugen und Frameworks unterstützt, um semantische Anwendungen zu entwickeln und Wissen zu integrieren und abzufragen. Es ist eine wichtige Sprache im Bereich des Semantic Web und wird zur Modellierung von Ontologien und zur Entwicklung von semantischen Anwendungen in vielen Bereichen der Erdsystemwissenschaften, des Wissensmanagement, des E-Commerce und des E-Learning eingesetzt.

**Kurz erklärt: SPARQL Protocol And RDF Query Language.**

Mit SPARQL können komplexe Abfragen auf RDF-Daten ausgeführt werden, um Informationen zu extrahieren, Beziehungen zwischen Ressourcen zu analysieren und komplexe Muster innerhalb der Daten zu identifizieren.

SPARQL verwendet eine Syntax, die an SQL erinnert, aber speziell für die Abfrage von RDF-Daten angepasst wurde. Die Abfragen bestehen aus verschiedenen Klauseln, wie z.B. SELECT, WHERE, OPTIONAL, FILTER, GROUP BY und ORDER BY. Diese Klauseln ermöglichen es, bestimmte Ressourcen oder Beziehungen innerhalb der Daten zu identifizieren und miteinander zu verknüpfen.

Zum Beispiel könnte eine SPARQL-Abfrage lauten: *"SELECT ?name WHERE {?person rdf:type foaf:Person. ?person foaf:name ?name. FILTER regex(?name, 'John', 'i')}"*

Diese Abfrage würde alle Namen von Personen im RDF-Graph zurückgeben, deren Name das Wort "John" enthält.

SPARQL wird häufig verwendet, um Daten aus Linked Data-Quellen abzufragen und zu integrieren. Es wird von vielen Semantic-Web-Tools und Semantic-Web-Frameworks unterstützt und kann ebenfalls verwendet werden, um komplexe Anwendungen und Dienste zu entwickeln, die auf semantischen Daten basieren.

**Kurz erklärt: GEOSPARQL**

GEOSPARQL ist eine Erweiterung der SPARQL-Abfragesprache, die entwickelt wurde, um die Abfrage und Verarbeitung von geografischen Informationen auf Grundlage von RDF-Daten zu ermöglichen. Konkret können mit GEOSPARQL komplexe räumliche Abfragen auf RDF-Daten um geografische Informationen zu extrahieren und räumliche Beziehungen zwischen den Ressourcen zu analysieren. Es ermöglicht die Darstellung und Abfrage von Punkten, Linien, Polygonen und anderen geometrischen Objekten.

Die Syntax von GEOSPARQL ähnelt der von SPARQL, enthält jedoch spezifische geografische Funktionen und Operationen.  Sie bietet eine Reihe von Operatoren, wie z.B. Intersect, Within, Contains, Distance usw., die verwendet werden, um räumliche Beziehungen zwischen Geometrien zu überprüfen.

Ein Beispiel für eine Geosparql-Abfrage könnte wie folgt aussehen:

>*"PREFIX geo: <http://www.opengis.net/ont/geosparql#>*<br>
>*SELECT ?name WHERE {*<br>
>> *?place geo:hasGeometry ?geometry.*<br>
>> *?geometry geo:asWKT ?wkt.*<br>
>> *FILTER(geo:sfWithin(?wkt, 'POLYGON((-122.5 37.5, -122.5 38.5, -121.5 38.5, -121.5 37.5, -122.5 37.5))')).*<br>
>> *?place foaf:name ?name.*<br>
>*}"*

Diese Abfrage sucht nach Orten im RDF-Graph, deren Geometrie innerhalb eines bestimmten geografischen Bereichs liegt. Es verwendet die Geosparql-Präfixe und die Funktion "geo:sfWithin", um die räumliche Beziehung zu überprüfen. Die Ergebnisse der Abfrage sind die Namen der entsprechenden Orte.

### 2.4 Inhaltliche Vertiefung - Beispiele aus der Praxis

**Kurz vorgestellt: WikiData**

Wikidata ist eine kollaborative, offene Wissensdatenbank, die von der Wikimedia Foundation entwickelt wurde. Sie wurde im Jahr 2012 gestartet und hat das Ziel, strukturierte Daten zu erfassen und bereitzustellen, die von allen genutzt werden können. Wikidata ist eine zentrale Wissensquelle, die von verschiedenen Wikimedia-Projekten wie Wikipedia, Wikimedia Commons und anderen genutzt wird.

Wikidata besteht aus einer Vielzahl von Einträgen, die Informationen über verschiedene Konzepte, Entitäten und Objekte enthalten. Jeder Eintrag in Wikidata repräsentiert eine spezifische Entität, wie zum Beispiel eine Person, einen Ort, ein Kunstwerk oder ein wissenschaftliches Konzept. Diese Entitäten werden mit eindeutigen Identifikatoren, den sogenannten Wikidata-IDs, gekennzeichnet.

Die Daten in Wikidata sind strukturiert und basieren auf semantischen Wissensmodellen. Das bedeutet, dass die Informationen in einer standardisierten Form vorliegen und Beziehungen zwischen den Entitäten durch verlinkte Daten hergestellt werden. Wikidata verwendet das RDF-Datenmodell und ermöglicht die Verknüpfung von Einträgen mit anderen Wissensquellen und externen Datenbanken.

Benutzer können Informationen zu Einträgen hinzufügen, bearbeiten und aktualisieren. Dadurch entsteht eine kollaborative Umgebung, in der das Wissen kontinuierlich erweitert und verbessert wird. Durch die Nutzung von IDs wird es ermöglicht, mehrsprachige Informationen zu speichern und über eine eigene API wird der externe Zugriff auf die Daten ermöglicht.

Durch die Nutzung von Wikidata können Anwendungen und Dienste auf eine große Anzahl von strukturierten Daten zugreifen und diese für ihre Zwecke verwenden. Das Projekt trägt zur Förderung des offenen Wissensaustauschs und der Vernetzung von Informationen bei.

**Kurz vorgestellt: Semantische Technologien im Kontext von INSPIRE**

INSPIRE (Infrastructure for Spatial Information in the European Community) ist eine Initiative der Europäischen Union, die darauf abzielt, eine harmonisierte Infrastruktur für räumliche Informationen zu schaffen und den Austausch von geografischen Daten und Informationen in Europa zu erleichtern. INSPIRE verwendet die folgenden semantischen Technologien und Strukturen, um die Interoperabilität und den Austausch von geografischen Informationen zu erleichtern:

**1. Ontologien und Schemata:**
INSPIRE definiert ontologische Modelle und Schemata, die eine einheitliche und konsistente Modellierung von geografischen Daten ermöglichen. Diese ontologischen Modelle beschreiben die Bedeutung und Beziehungen von Konzepten in verschiedenen Themenbereichen, wie z.B. Gewässer, Geologie oder Landnutzung. Durch die Verwendung gemeinsamer ontologischer Modelle wird eine einheitliche Interpretation und Integration von geografischen Daten über verschiedene Quellen hinweg ermöglicht.

*Ein konkretes Beispiel ist die INSPIRE-Themenschicht "Schutzgebiete". Hier wird eine Ontologie entwickelt, die die verschiedenen Arten von Schutzgebieten, wie Naturschutzgebiete, Natura 2000-Gebiete oder Vogelschutzgebiete, sowie deren hierarchische Beziehungen und Eigenschaften beschreibt. Durch die Anwendung dieser ontologischen Modelle können die Schutzgebietsdaten verschiedener Länder oder Organisationen interoperabel und einheitlich interpretiert werden.*

**2. Harmonisierte Metadaten:**
INSPIRE legt Standards für die Beschreibung von Metadaten fest. Metadaten beschreiben Informationen über geografische Datensätze, wie z.B. ihre Herkunft, Qualität und räumlichen Ausdehnung. Die Verwendung von semantischen Technologien ermöglicht die präzise Beschreibung und Strukturierung dieser Metadaten, was wiederum die Suche, den Zugriff und den Austausch von geografischen Informationen erleichtert.

*Ein Beispiel ist die Verwendung des INSPIRE-Metadatenschemas für Geodäsie. Es definiert eine strukturierte Beschreibung von Geodaten, wie geodätische Referenzsysteme, Koordinatenreferenzsysteme und Transformationen. Durch die semantische Strukturierung der Metadaten wird es einfacher, Informationen über geodätische Daten aus verschiedenen Quellen zu verstehen, zu vergleichen und zu kombinieren.*

**3. Verknüpfung und Integration von Daten:**
INSPIRE fördert die Verknüpfung und Integration von geografischen Daten aus verschiedenen Quellen. Durch die Verwendung von semantischen Technologien können geografische Daten miteinander verknüpft werden, indem semantische Beziehungen und Verbindungen zwischen den Daten hergestellt werden. Dies erleichtert die Kombination und Integration von Daten aus verschiedenen Quellen und ermöglicht so eine umfassendere und kontextbezogene Nutzung der Informationen.

*Ein Beispiel ist die Verknüpfung von Geodaten zu Umweltthemen wie Luftqualität oder Gewässerqualität. Durch die semantische Verknüpfung können Luftqualitätsdaten mit Informationen über Standorte von Umweltmessstationen, geografischen Merkmalen wie Straßen oder Grünflächen und geografischen Merkmalen in der Nähe von Gewässern in Beziehung gesetzt werden. Dies ermöglicht eine bessere Analyse und Verständnis der Auswirkungen von Umweltfaktoren auf die Luft- und Wasserqualität.*

**4. Semantische Abfragen und Analysen:**
INSPIRE unterstützt semantische Abfragen und Analysen von geografischen Daten. Durch die Verwendung von semantischen Technologien wie SPARQL können komplexe Abfragen gestellt werden, um spezifische Informationen aus den geografischen Datenbeständen abzurufen. Dies ermöglicht eine präzisere und effizientere Suche nach räumlichen Informationen und unterstützt Entscheidungsprozesse und Analysen, die auf geografischen Daten basieren.

*Beispielsweise könnte durch eine Abfrage die Suche nach Straßenabschnitten mit bestimmten Verkehrsdichten, die nahe bestimmter Verkehrsknotenpunkte liegen durchgeführt werden. Dies ermöglicht eine präzise Analyse von Verkehrsdaten und unterstützt Verkehrsplanung und -managemententscheidungen.*

Durch die Anwendung semantischer Technologien und Strukturen fördert INSPIRE die Harmonisierung, Integration und effiziente Nutzung von geografischen Informationen auf europäischer Ebene. Diese semantischen Ansätze tragen dazu bei, die Interoperabilität von geografischen Daten zu verbessern und ermöglichen eine umfassendere Nutzung der Informationen für verschiedene Anwendungen und Entscheidungsprozesse.

### 2.5 Inhaltliche Vertiefung - Die Vision auf dem Prüfstand

**Die Vision eines Semantic Webs auf dem Prüfstand - Wie weit sind wir denn eigentlich?**

Die Vision des Semantischen Web wurde bereits vor mehr als 20 Jahren von Tim Berners-Lee, dem Erfinder des World Wide Web, vorgestellt. Seitdem wurden viele Fortschritte gemacht, aber die vollständige Realisierung der Vision ist noch immer nicht erreicht worden.

Einige Fortschritte und Technologien, die zum Semantischen Web beitragen, sind bereits vorhanden. Dazu gehören das Resource Description Framework (RDF), die Web Ontology Language (OWL) und SPARQL als Abfragesprache für das Semantische Web. Diese Technologien ermöglichen es, Informationen im Web semantisch anzureichern und miteinander zu verknüpfen.

Es gibt auch verschiedene Anwendungen und Initiativen, die das Semantische Web nutzen. Beispielsweise werden semantische Technologien in Bereichen wie der medizinischen Forschung, der digitalen Bibliothekswissenschaft, dem E-Commerce und der Wissensmanagement-Systeme eingesetzt.

Einige spezifische Beispiele für semantische Anwendungen sind semantische Suchmaschinen, die eine genauere und kontextbezogene Suche ermöglichen, semantisch angereicherte Inhalte, die maschinenlesbar sind und automatische Datenintegration ermöglichen, und intelligente Assistenten, die natürliche Sprache verstehen und relevante Informationen liefern können.

Allerdings gibt es auch Herausforderungen und Hindernisse, die einer breiteren Umsetzung des Semantischen Webs im Wege stehen. Ein zentrales Problem besteht darin, dass die semantische Anreicherung von Informationen auf Webseiten noch nicht weit verbreitet ist. Viele Webseiten enthalten nach wie vor unstrukturierten Text, der von Maschinen schwer interpretiert werden kann.

Darüber hinaus besteht die Herausforderung, große Mengen an Daten aus verschiedenen Quellen zu integrieren und zu harmonisieren. Das Semantische Web erfordert eine einheitliche Modellierung von Daten und eine Konsensbildung über die Bedeutung von Begriffen und Beziehungen.

Ein weiteres Hindernis ist die Akzeptanz und Adaption der semantischen Technologien. Viele Entwickler und Organisationen sind mit den herkömmlichen Webtechnologien vertraut und möglicherweise nicht ausreichend geschult oder motiviert, auf semantische Ansätze umzusteigen.

Insgesamt lässt sich sagen, dass das Semantische Web trotz der Fortschritte noch nicht in vollem Umfang verwirklicht ist. Es bleibt eine Herausforderung, die Vision des Semantischen Webs umfassend umzusetzen und eine breite Akzeptanz sowohl bei Entwicklern als auch bei Nutzern zu erreichen. Dennoch gibt es weiterhin Bemühungen und Entwicklungen in diese Richtung, sodass das Potenzial des Semantischen Webs auch weiterhin erforscht und genutzt wird.

## 3. Übungen und Leitfäden

**Aufbau der Übungen und Leitfäden**
* Aufgabenstellung 
* Videoguide (Screencast)

### 3.1 Übung 1

**Aufgabenstellung**

In dieser Übung beschäftigen wir uns mit Hilfe des Webtools "WebVOWL" mit dem Thema Ontologien. Wir werden zunächst beispielhafte Graphen sichten und im Anschluss selbst eine simple Ontologie zu einem ausgewählten Thema erstellen. 

Folge dem Screencast und erstelle nach dem gleichen Prinzip eine oder auch mehere Ontologien zu Themenbereichen die dich besonders interessieren. 

**Skript zum Videoguide**

**WebVOWL** ist ein benutzerfreundliches Online-Tool, das uns hilft, OWL Ontologien zu visualisieren und interaktiv zu erforschen. Es ermöglicht uns komplexe Zusammenhänge und Strukturen in einer Ontologie anschaulich darzustellen.

Wenn wir WebVOWL öffnen, sehen wir zunächst zwei Fenster. Im Hauptfenster sehen wir eine Visualisierung eines interaktiven Graphen, der eine OWL Ontologie darstellt. Es ist möglich zu zoomen, einzelne Elemente des Graphen auszuwählen und sich frei auf der Oberfläche zu bewegen. Im rechten Fenster befindet sich eine Infobox, in dieser Infobox ist unter anderem der Titel der dargestellten Ontologie, sowie eine Kurzbeschreibung zu finden. Zusätzlich erscheinen hier Informationen zu Metadaten oder Statistiken. Sobald ein Element in der Grafik ausgewählt wird, erscheinen unter dem Menüpunkt „Selection Details“ detaillierte Informationen zu diesem Element.

Im unteren Bereich der Seite befindet sich eine Leiste mit verschiedenen Menüpunkten:

Über die Suchleiste können Elemente des Graphen über ihre Beziehungen gesucht werden.

Unter „Ontology“ finden sich beispielhafte Ontologien zur Orientierung, es können aber auch weitere Ontologien geladen oder neu erstellt werden.

Über den Menüpunkt „Export“ können die erstellten Ontologien in verschiedenen Formaten gespeichert oder als URL zur Verfügung gestellt werden.

Der Menüpunkt „Filter“ ermöglicht es, einzelne Inhalte in der Visualisierung auszublenden, um die Übersichtlichkeit zu erhöhen und sich auf das Wesentliche konzentrieren zu können.

Der Menüpunkt „Optionen“ mit einigen Einstellungsmöglichkeiten zu Zoomstufen, Beschriftungsgrößen oder Abständen zwischen den Knoten trägt ebenfalls zur Übersichtlichkeit der Visualisierung bei.

Über den Punkt „Modes“ kann der Bearbeitungsmodus auf Edit umgeschaltet werden, der das Hinzufügen oder Ändern von Graphelementen erst ermöglicht.

Sobald der Bearbeitungsmodus eingeschaltet ist, wird unter dem übergeordneten Menüpunkt „Ontology“ der Punkt „Create New Ontology“ nutzbar. Damit kann eine eigene Ontologie erstellt werden.

Im rechten Fenster können wir einen Titel für unsere Ontologie festlegen und da unsere selbst erstellte Ontologie den Tourismus in verschiedenen Ländern behandeln soll, wählen wir den Titel „Tourismus“. Auf der linken Seite finden wir die Default Elements „Class“, „Property“ und „Datatype“, aus denen wir unseren Graphen zusammensetzen können.

Kurze Übersicht Default Elements:

*Kurze Übersicht Default Elements:
„OWL:Thing“ ist ein grundlegendes Konzept in OWL und repräsentiert alle möglichen Instanzen Entitäten in einer Ontologie. Es stellt den obersten Punkt in der Klassenhierarchie dar und umfasst alles was in der Ontologie existieren kann.
* „OWL:Class“ ist ein Konzept in OWL, das eine Klasse in der Ontologie repräsentiert. Klassen werden verwendet, um Konzepte, Objekte oder Entitäten innerhalb einer Domäne zu repräsentieren.
* „OWL:DeprecatedClass“ ist eine Markierung in OWL, die angibt, dass eine Klasse veraltet ist oder nicht mehr empfohlen wird. 
* „OWL:ObjectProperty“ ist eine Eigenschaft in OWL, die Beziehungen zwischen Objekten in einer Ontologie beschreibt. Sie definiert, dass die Werte der Eigenschaften andere bekannte Individuen oder Klassen sind.
* „OWL:SubClassOf“ ist eine Beziehung in OWL, die angibt, dass eine Klasse eine Unterklasse einer anderen Klasse ist.
* „OWL:DisjointWith“ ist eine Beziehung in OWL, die angibt, dass zwei Klassen keine gemeinsamen Instanzen haben und sich gegenseitig ausschließen.
* „OWL:AllValuesFrom“ ist eine Einschränkung in OWL, die besagt, dass alle Werte, die mit einer Eigenschaft assoziiert sind, zu einer bestimmten Klasse gehören müssen.
* „OWL:SomeValuesFrom“ ist eine Einschränkung in OWL, die besagt, dass mindestens einer der mit einer Eigenschaft assoziierten Werte zu einer bestimmten Klasse gehören muss.
* Unter „Datatype“ finden wir klassische Datentypen wie String, Integer oder Double, mit denen definiert werden kann, in welcher Form die jeweiligen Klassen vorliegen können. 

In unserer Ontologie fügen wir als erstes die drei Klassen Stadt, Land und Sehenswürdigkeiten hinzu, dazu klicken wir auf OWL:Class und mit einem Doppelklick werden die Klassen hinzugefügt. Falls zu viele Klassen hinzugefügt wurden, können diese einfach über das rote X wieder gelöscht werden. Durch Anklicken der Klassen können diese benannt werden. Über das grüne X können wir den Klassen Datentypen zuordnen, die wir in der linken Spalte auswählen.

Als nächstes definieren wir erste Beziehungen zwischen den erstellten Klassen. Wir definieren, dass eine Stadt eine Unterklasse eines Landes ist. Dazu wählen wir „OWL:SubClassOf“ und ziehen mit dem angezeigten Pfeil eine Verbindung von der Klasse Stadt zu Land.

Als nächstes erstellen wir drei Klassen, die die Länder repräsentieren, in unserem Beispiel Deutschland, Italien und England. Diese Klassen verbinden wir alle als Unterklassen mit der Klasse Land. Außerdem erstellen wir drei Klassen, die die Hauptstädte der ausgewählten Länder repräsentieren. Diese werden dann zunächst als Unterklassen mit der Klasse Stadt verbunden. 

Da Berlin aber nicht nur eine Stadt, sondern auch die Hauptstadt von Deutschland ist, können wir eine „ObjektProperty“ verwenden, um die Verbindung zwischen dem Land und der Hauptstadt herzustellen. Dazu erstellen wir eine Verbindung vom Land zur jeweiligen Hauptstadt und beschreiben diese Verbindung als Hauptstadt.

Diese Schritte müssen nun für die Sehenswürdigkeiten der Städte wiederholt werden. Diese können nun selbst erstellt werden.


### 3.2 Übung 2

**Aufgabenstellung**

In dieser Übung beschäftigen wir uns damit SPARQL-Abfragen in der semantischen Datenbank WikiData anzuwenden. Wir schauen uns die Struktur einiger beispielhaften Abfragen und deren Ergebnisse in der Wikidata-Query an. Anschließend erstellen wir mithilfe des Query-Builders Eine eigene einfache Abfrage.

Folge dem Screencast und nutze die vorgestellten Ressourcen gerne um weitere Abfragen zu erstellen und durchzuführen.

**Skript zum Videoguide**


## 4. Quiz

**Fragen**

* Wer ist der Erfinder des World Wide Web und Semantic Web?

* Ordne den Jahreszahlen ihre Entwicklungen zu

* Für wen soll das Semantic Web Informationen im Internet verständlicher machen?

* Beim Linked Data Konzept muss der Benutzer den genauen Speicherort der Daten kennen!

* Beim Knowledge Graphen Konzept wird das Resource Description Framework(RDF) als Datenmodel genutzt!

* Knowledge Graph kann Informationen aus Quellen wie APIs, unstrukturierten Texten, stukturierten Datenbanken und verschiedenen Webseiten zusammenführen!

* Ziehe die Wörter in die richtigen Felder!

* Welche drei Komponenten gibt es im RDF-Model?

* Web Ontology Language (OWL) wird verwendet, um komplexe Ontologien zu definieren, also hierarchische und semantische Strukturen, die Wissen und Beziehungen zwischen Konzepten repräsentieren!

* GEOSPARQL ermöglicht die Abfrage auf RDF-Daten von was?

* Welche Rolle spielt Wikidata in der Wissensvernetzung im Web?

* Von welcher Organisation ist INSPIRE?

## 5. Zusammenfassung

Hey das hast du gut gemacht! Wir hoffen, dass du nun eine Vorstellung davon hast, was Knowledge Graphen, das Semantic Web und Linked Data sind und wie diese Wissensmodellierungen im Kontext von Geodateninfrastrukturen eingesetzt werden können.

**Interessiert daran, mehr zu lernen?**

Im Internet findest du eine Fülle von Lern-Ressourcen zum Thema der Wissensmodellierung in Form von Knowledge Graphen, dem Semantic Web und Linked Data. Hier sind einige Empfehlungen:

* ["The semantic web" paper by Berners-Lee et al. (2001)](https://www-sop.inria.fr/acacia/cours/essi2006/Scientific%20American_%20Feature%20Article_%20The%20Semantic%20Web_%20May%202001.pdf)
* [Tim Berners-Lee's TED Talk on Linked Data](https://www.youtube.com/watch?v=OM6XIICm_qo)
* [EO4GEO: Ontologies development reuse and patterns](https://bok.eo4geo.eu/WB2-3)
* [Wikidata Introduction: How does Wikidata work?](https://www.wikidata.org/wiki/Wikidata:Introduction)
* Harvey, F., et al. "Semantic interoperability: A central issue for sharing geographic information." The annals of regional science 33.2 (1999): 213-232.
* Kuhn, W. "Geospatial semantics: why, of what, and how?." Journal on data semantics III. Springer, Berlin, Heidelberg, 2005. 1-24.

**Dein Feedback ist willkommen!**

Wenn du Unzulänglichkeiten in diesem OER-Modul festgestellt oder Ideen zur Verbesserung des OER-Materials hast, bist du herzlich dazu eingeladen Einträge in die Problemliste im [GitHub-Repositorium](https://github.com/oer4sdi) dieses OER hinzuzufügen.
