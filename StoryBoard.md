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
*Eine URL enthält das Schema (z. B. "http://"), gefolgt von der Domain (z. B. "www.example.com") und dem Pfad zur spezifischen Ressource (z. B. "/pfad/zur/datei.html").*

Ein weiterer Typ ist der Uniform Resource Name (URN), der dazu dient, Ressourcen unabhängig von ihrem aktuellen Speicherort dauerhaft und eindeutig zu identifizieren. URNs können verwendet werden, um zum Beispiel auf bibliografische Informationen, Dokumente oder andere digitale Objekte zu verweisen.

URIs spielen eine zentrale Rolle im Web, da sie die Grundlage für das Adressieren und Verlinken von Ressourcen bilden. Durch die Verwendung von URIs können Benutzer und Maschinen auf die gewünschten Ressourcen zugreifen, sei es durch das Eingeben der URI in einen Webbrowser oder durch das Klicken auf Hyperlinks, die auf URIs verweisen.

Es ist wichtig anzumerken, dass URLs und URNs eng miteinander verwandt sind und beide als Untergruppe von URIs betrachtet werden können. URLs dienen jedoch hauptsächlich dazu, Ressourcen zu lokalisieren, während URNs auf ihre Identität abzielen.

**Kurz erklärt: Resource Desciption Framework**

RDF (Resource Description Framework) ist ein Datenmodell des Semantic Web, das verwendet wird, um strukturierte Informationen über Ressourcen im Web zu beschreiben und zu verlinken.

Das RDF-Modell besteht aus drei grundlegenden Komponenten: Ressourcen, Eigenschaften und Werten. Eine Ressource wird durch eine URI (Uniform Resource Identifier) identifiziert und repräsentiert eine Entität im Web wie z.B. eine Person, ein Ort oder ein Dokument. Eine Eigenschaft (auch Prädikat genannt) beschreibt eine Beziehung zwischen zwei Ressourcen und wird ebenfalls durch eine URI identifiziert. Ein Wert gibt an, welcher Wert die Eigenschaft für die Ressource hat, die sie beschreibt.

RDF-Daten werden in Tripeln ausgedrückt, die aus einem Subjekt, einem Prädikat und einem Objekt bestehen. Das Subjekt ist die Ressource, auf die sich das Tripel bezieht, das Prädikat beschreibt die Beziehung zwischen dem Subjekt und dem Objekt, und das Objekt ist der Wert, der die Beziehung beschreibt. Die Tripel werden auch als "Sätze" oder "Statements" bezeichnet.

Ein Beispiel für ein RDF-Tripel könnte lauten:*"Tim" besitzt das Attribut " hat Alter" mit dem Wert "30". In diesem Fall ist "Tim" das Subjekt, "hat Alter" das Prädikat und "30" das Objekt.*

RDF ermöglicht es, komplexe Beziehungen zwischen Ressourcen im Web auszudrücken und zu verknüpfen, wodurch das Web zu einem globalen Wissensraum wird.




