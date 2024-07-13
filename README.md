# La Mediterranea - Entwicklung eines Online-Tischreservierungssystems

Prüfungsbewerber : Hiba, Irina, Puya und Heiko

## 1. Projekteinführung

Die folgende Projektdokumentation wurde im Rahmen der Umschulung als virtuelles Laborprojekt erstellt,
welches die Verfasser während Iherer Umschulung zur Fachinformatikerin /zum Fachinformatiker Anwendungsentwicklung
solbstständig durchgeführt hat. Inititator und Projektbegleiter war unser Dozent Dr. Holger Kramer - welcher uns im Projektmanagement, in der Programmierung von Python und der objektorierntierten Programmierung unterrichtet.

### 1.1 Projektumfeld

Das multilinguale und multikulturelle Entwicklerteam aus 4 Nationen ist spezialiesiert auf individuelle
Kundenlösungen in der Gastronomie und der Veranstaltungstechnik. Im Angebot befinden sich Lösungen für
Bars, Restaurants, Diskotheken und Veranstaltungen wie Konzerte oder DJ-Events.

### 1.2 Projektumsetzung

Die Projektumsetzung fand online statt, die Projektteilnehmer nutzen Microsoft Teams und GitHub zur
gemeinsamen Durchführung der Programmiertätigkeiten. Sämtliche Programmiertätigkeiten sowie Tests
und Anpassungen wurden durch Hiba, Irina, Puya und Heiko durchgeführt.

### 1.3 Projektziel

Es soll eine Anwendung zur Verfügung gestellt werden, in welcher sich Kunden auf einfache Weise
über die Website des Auftraggebers einen Tisch im Restaurantsbereich reservieren können. Zusätzlich
sollen die Reservierung über eine App auf dem Restaurant-Desktop über entsprechende Masken bearbeitet
werden können. Dieses Ziel erfordert eine neu entwickelte Software mit Benutzeroberfläche und entsprechender
Auswahl- und Bearbeitungsmöglichkeit (Web und App) für die Benutzer.

## 2. Projektanalyse

### 2.1 Ist-Analyse

Die Reserverierungen werden analog (per Telefon/Im Restaurant) entgegengenommen und auf einem Papierkalender
im Empfangsbereich eingetragen. Hierdurch ist die Bearbeitung der Reservierungen nur an diesem zentralen Platz möglich.

### 2.2 Soll-Analyse

Mit einem Online-Reservierungssystem soll eine Terminerfassung bzw. Vergabe sowohl von Kunden als auch
Mitarbeitenden dezentral möglich sein. Hierzu soll die Software die Möglichkeit bieten, verfügbare Plätze
auswählen zu können dieses zu reservieren und auch zu stornieren.

### 2.3. Projektbegründung

Die Kunden von La Meditteranea können ausschließlich per Telefon oder im Gespräch mit den Mitarbeitenden
Reservierungen durchführen. Reservierungen sind daher nur während der Öffnungszeiten möglich.

Durch die Softwarelösung können nun sowohl Kundinnen und Kunden als auch die Mitarbeitenden rund um die
Uhr und an jedem Tag der Woche sowohl Reservierungen vornehmen als auch bearbeiten bzw. stornieren.

Durch die zentrale Speicherung in einer Datenbank können die Daten sowohl gesichert als auch von den
Mitarbeitenden ausgewertet werden. Wichtigste Verbesserungen sind hier die ständige Verfügbarkeit
der Reservierungsmöglichkeit, die Zeit- und Aufwandseinsparung bei den Mitarbeitenden und eine
Sicherung der Reservierungsdaten. Die gute Kundenbindung soll verbessert werden und neue Kundinnen
und Kunden gewonnen werden. Anhand der Daten kann zukünftig ein "Customer-Relation-Management-System"
entwickelt werden.

### 2.4. "make or buy"-Entscheidung

Bei diesem Projekt handelt es sich um eine Individuallösung. Nachdem diverse Tools und Programme
zum Reservieren getestet und verglichen wurden, wurde sich aus wirtschaftlichen und individuellen Gründen
für eine Eigenentwicklung entschieden. Die getesteten Tools entsprachen nicht den Vorstellungen an
die Anpassbarkeit und Auswertungsmöglichkeiten, welche gewünscht waren und wären daher auch finanziell
gesehen nicht sinnvoll gewesen. Ein großer Vorteil ist hierbei auch die individuell anpassbare
Schnittstelle zur internen MySQL-Datenbank, welche bereits die Inhalte für die Website ausliefert.

## 3 Projektplanung

### 3.1. Projektphasen

Dem Projektteam stehen analog den IHK Vorgaben 80 Stunden Arbeitszeit pro Person zur Verfügung.
Die Durchführung des Projektes findet innerhalb des ersten Jahres der Umschulung statt. Die Stunden werden über diesen Zeitraum verteilt, da "im Tagesgeschäft" mehrere Unterrichtseinheiten absolviert werden und dadurch zusätzliche Projekte bearbeitet werden müssen.

|Projektphase|Geplante Dauer in Stunden|
|---|---|
|Analysephase|24|
|Planungsphase / Entwurfsphase|32|
|Entwicklungsphase|216|
|Testphase|16|
|Fehleranalyse|8|
|Vorstellung und Abnahme|4|
|Projektdokumentation|20|
|__Gesamtdauer__|__320__|

### 3.2 Ressourcenplanung

Die Projektumsetzung fand unter online unter Nutzung von Microsoft Teams und GitHub sowie den Endgeräten der Umschulenden Hiba, Irina, Puya und Heiko statt.

Als installierte Betriebssysteme wurden Windows 11 Professional, MacOS X und Ubuntu-Linux in den jeweils aktuellen Versionen eingesetzt.

Zur Entwicklung wurde eine Python-, MySQL-, HTML-, PHP- und CSS-fähige Entwicklungsplattform benötigt, verwendet wurde Microsoft Visual Studio Code in der aktuellsten Verison.

Bei der verwendeten Software und den Plugins sowie Frameworks wurde darauf geachtet, dass diese
kostenlos zur Verfügung stehen bzw. sowieso schon lizenziert sind oder eingesetzt werden.
So entstanden den Umschulenden durch die Entwicklung der Software keine zusätzlichen Kosten.

### 3.3 Zielplattformen

Als Zielplattformen wurde Microsoft Windows 11 gewählt, da alle vorhanden PCs in der Bar/dem Restaurant mit Windows 11 als Betriebssystem arbeiten. Die Nutzung der Weboberfläche ist Plattformunabhängig.

Optional ist eine Umsetzung auf die gängige weitere Betriebssysteme wie MacOS, iOS, Linux, Android.

Als Programmiersprachen wurde sich für Python, PHP, HTML, CSS und (My)SQL entschieden, da für dies Programmiertätigkeiten bereits genug know-how vorhanden bzw. aktuell im Aufbau ist. 

Mit den gewählten Programmiersprechen und der MySQL-Datenbank können alle erforderlichen und gewünschten Ziele umgesetzt werden. Erstellt wurde das Projekt als Desktop-App mit der Python 3.12.4 und als Web-App mit PHP 8.20.

### 3.4 Architekturdesign

Das Projekt basiert auf dem Architekturprinzip MVC (Model-View-Controller). Die Software lässt sich gemäß diesem Muster in die drei Bereiche Model (Datenaufbereitung), View (Präsentation) sowie Controller (Anwendungssteuerung) unterteilen. Aus dieser Trennung ergeben sich einige Vorteile wie bessere Wartbarkeit, Lesbarkeit und Erweiterbarkeit. Da die Logik von der Darstellung getrennt ist, kann man etwa die Oberfläche leicht austauschen, ohne tiefer in den logischen Bereich der Software vordringen zu müssen.

## 4. Projektentwicklung

### 4.1 Datenerhebung

#### 4.1.1 Datenermittlung

Auf Basis der vorliegenden analogen Daten aus alten Kalendern wurde sich ein grober Überblick über die bisher vorliegenden Kundendaten verschafft. Bisher liegen nur Daten wie Vor- und Nachname aus der Vergangenheit vor.

#### 4.1.2 Datenbankanalyse

Die Analyse der Kundenddaten gestalte sich aufwendiger, da diese nur in analoger Form von handschriftlichen Kalendereinträgen vorlagen. In der zu entwickelnden Datenbank soll zukünftig die eMail-Adresse als Eineindeutiger Identifikator verwendet werden und eine Kundennummmer als UniqueID automatisch generiert werden.

### 4.2 Datenbankentwicklung

* ERM-Model
* Design
* Umsetzung

### 4.3 SQL Abfrage konzipieren und als PHP-Script in besthehnde Website integrieren

Für die zu entwickelnde Datenbank sind die vorhandenen HTML-Seiten auf PHP umzustellen
und die Abfragen in diese zu integrieren.

### 4.4 Anwendungsentwicklung mit Python

#### 4.4.1 Modellierung, Klassen etc. erstellen

* UML Diagramme erstellen (Klassendiagramm, Aktivitätsdiagramme, PAP)

#### 4.4.2 Entwurf der Benutzeroberfläche erstellen

* GUI unter Benutzung des Moduls Tkinter? erstellen

#### 4.4.3 Entwicklung der Form und Methoden

* Beim Start der App soll direkt eine Übersicht der aktuellen Reservierungen angezeigt werden

* Beim Aufruf der Reservierungs-Seite auf der Website soll eine auf die Kundensicht angepasste Übersicht der Reservierungsmöglichkeiten angezeigt werden.

#### 4.4.? Benutzerfreundlichkeit

* Zum Zecke der Benutzeroberfläche wurde nach Rückmeldung der Anwender noch an Versserungen der Eingabemasken garbeitet.

### 4.5 Qualitätsmanagement

#### 4.5.1 Testphase

Der Großteil der Testphase wurde vom Entwicklerteam selbst vorwiegend während der Entwicklungsphase
in White-Box-Tests durchgeführt. Nach Fertigstellung der Anwendung fanden Black-Box-Tests durch
weitere Umschülerinnen und Umschüler so wie Freunde, Bekannte und Familienmitglieder statt, welche 
aber keine weiteren Programmfehler zu Tage förderten.

#### 4.5.2 Fehleranalyse / -Korrektur

Da die Software von den Autoren bereits während der Entwicklung regelmäßig geprüft und korrigiert wurde,
fällt dieser Punkt recht knapp aus. Gründe für Abstürze wurden während der Entwicklungszeit fortwährend behoben,
während der Testphase liefen sowohl die Windows-Desktop-App als auch die Web-App recht stabil.

...

## 5. Abschuluss

### 5.1 Soll-/Ist-Vergleich

Die Projektdauer konnte im Großen und Ganzen eingehalten werden, im Detail der veranschlagten Zeitplanung gab es wie
erwartet Abweichungen. Dadurch, dass während des Entwicklungsprozesses Material aus den Aufgaben im Unterreicht
verwendet werden konnte und bereits viel getestet wurde, verschob sich der anteilige Zeitbedarf von der reinen
Testphase hin zur Entwicklungs- und Dokomentationsphase.

### 5.2 Kosten- und Nutzenanalyse

Eine Kosten- und Nutzenrechnung sowie eine Amortisationsrechnung können in diesem Fall nicht erstellt
werden. Kosten für das Projekt werden mit den investierten Arbeitsstunden außerhalb der normalen
Umschulungszeiten in Relation gesetzt und Preise werden nicht kalkuliert, da es sich um ein reine
Labor-Projekt handelt. Auch dadurch, dass man den Mehrwert im Vergleich zur vorhergehenden Arbeitsweise
nicht direkt in Zahlen gemessen werden kann, wird auf diese Rechnungen verzichtet.

Der Nutzen des Online-Reservierungssystem liegt ganz in einer höheren Verfügbarkeit (24h/7d) für Kundinnen,
Kunden und Mitarbeitende.

### 5.3 Zukunftsausblick

Das Online-Reservierungssystem ist die Baisis für die Digitalierung, hieraus kann zukünftig eine Kundendatenbank
entwickelt werden um die Kunden z. B. durch Einwilligung zu einem Newsletter über aktuelle Entwicklungen (geänderte
Öffnungszeiten, aktualisierte Speisekarten und Angebote) zu informieren. Für das Projekt-Team ist damit die Basis
als "Blaupause" für die angestrebte IHK-Abschlussprüfung geschaffen.

## 6. Anhang

### 6.1 Glossar

### 6.2 Literaturverzeichnis

### 6.3 Darstellungsverzeichnis

### 6.4 Vergleich zwischen Zeitplanung und Zeitbedarf

### 6.5 Vergleich zwischen über Papierkalender verwelteten Reservierung und der mit Softwarelösung bearbeiteten Reservierungen

### 6.6 Benutzerdokumentation

### 6.7 ER- und UML-Diagramme

### 6.8 Quellcode