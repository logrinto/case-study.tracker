# Tracker

### Kommunikation
* [Zoom Meeting](https://zoom.us/j/214657003?pwd=TnFXQkhtNFdxME01K1hxNW9XLzVEZz09)
* Slack → [Channel #case-study](slack://channel?team=T6RSKS0PK&id=CNCQZFJF9)


## Ausgangslage
Es gibt auf dem Markt diverse so genannte «Tracking Tags». Dies sind kleine Geräte, welche den Standort des Geräts dem Besitzer mitteilen können. Der Benutzer und der Tag müssen dabei nicht am selben Ort sein. Somit eignet sich ein solches Gerät um zum Beispiel zu verfolgen wo ein Gepäckstück/Auto/… gerade ist.  
Es gibt diverse Anbieter von solchen Geräten und es gibt seit geraumer Zeit das Gerücht, dass Apple – als grosser Player – in diesen Markt einsteigen möchte.

* [Beispiel Tile](https://www.thetileapp.com/de-de/)
* [Beispiel Invoxia Roadie](https://www.invoxia.com/intl/gps-tracker)


## Aufgabe
Es soll eine Mobile-Applikation (App) entwickelt werden, welche dem User hilft einen Tracker in Betrieb zu nehmen (Registrierung), diesen zu konfigurieren und zu betreiben. Es handelt sich um eine native App und keine Website.
Die Aufgabe wird in fünf Gruppen ausgeführt.

### Zwischenpräsentation
Am 20. März 2020 um 11 Uhr muss ca. 5min. präsentiert werden, welche Funktionen man von der fertigen App erwarten kann. Also welche Funktionen sollen ermöglicht werden. Zu den Funktionen müssen mögliche Use Cases erarbeitet werden. Unter den gegebenen technischen Voraussetzungen könnten diverse Funktionen realisiert werden. Diese Zwischenpräsentation zeigt die ausgewählten Funktionen und deren Use Cases. Einstieg soll die Inbetriebnahme des Produkts sein (also nach dem Kaufprozess).
Die Zwischenpräsentation dient dem Lernprozess und soll einen Austausch innerhalb der Klasse fördern. Die Qualität des Entwurfs wird noch nicht beurteilt. 

### Präsentation
Um 15 Uhr müssen ca. 8min. die Interfaces zweier User Journeys präsentiert werden: «Onboarding» (Gerät in Betrieb nehmen) und eine Funktion anhand eines Anwendungsfalles (ergibt sich aus der Definition der Funktion vom Vormittag).
Zu visualisieren sind die relevanten Interface-Elemente. Die Präsentation muss auf [Github](https://github.com/logrinto/case-study.tracker/issues) hochgeladen werden.
  

## Funktionsmodel für Aufgabe
Das Gerät sendet den Standort nicht an das Gerät des Kunden, sondern an einen Server des Anbieters der immer verfügbar ist. Von dort können Daten von der App abgefragt werden.


```
                ┌───────────────────┐                
                │  Internet/Cloud   │                
                │                   │                
┌─────────────┐ │  ┌─────────────┐  │ ┌─────────────┐
│   Tacker    ◀─┼──▶   Server    ◀──┼─▶     App     │
└─────────────┘ │  └─────────────┘  │ └─────────────┘
                └───────────────────┘                
```


## Technische Fähigkeit
Das Tracking Gerät und die Infrastruktur dazu werden folgende technische Eigenschaften haben;

* Gerät hat eine Batterielaufzeit von 3 Monaten
* Gerät kann Standort via Mobilnetz (hat eigene bereits eingesetzte SIM-Karte) an Server senden
* Gerät kann vom Server die Nachricht erhalten, einen Ton zu spielen (kleiner Lautsprecher)
* App kann Push-Nachrichten vom Server empfangen
* App kann Standort-Verlauf vom Server abfragen
* Server kann Standort-Daten vom Tracker beliebig lange behalten (nur kleine Daten)
* Server kann Standort-Daten analysieren und Aktionen (Push-Nachrichten) auslösen


## Timetable
Pausen werden innerhalb der Gruppen selber koordiniert.

### Vormittag
* **8:15 – 8:45** Aufgabe eigenständig lesen. Kurze Recherche.
* **8:45 – 9:15** Aufgabe in Doppelklasse besprechen
* **9:15 – 11:00** Funktionen definieren und User Journey Map anlegen
  * **09:15 – 09:40** Michael & Stefan stehen bei Fragen zur Verfügung
  * **09:40 – 09:50** Gruppe 1 – Michael & Stefan geben Feedback
  * **09:50 – 10:00** Gruppe 2 – Michael & Stefan geben Feedback
  * **10:00 – 10:10** Gruppe 3 – Michael & Stefan geben Feedback
  * **10:10 – 10:20** Gruppe 4 – Michael & Stefan geben Feedback
  * **10:20 – 10:30** Gruppe 5 – Michael & Stefan geben Feedback
  * **10:30 – 11:00** Michael & Stefan stehen bei Fragen zur Verfügung
* **11:00 – 11:45** Jede Gruppe präsentiert ca. 5min. Funktion und Use Case

### Nachmittag
* **12:45 – 15:00** Jede Gruppe arbeitet an den Interfaces der App
  * **13:15** Jede Gruppe postet in Slack die wichtigsten «acceptance criteria», was die Applikation können muss. Dabei ist zu beachten, dass zwei User Journeys um 15 Uhr abgegeben werden müssen, die diese Kriterien abdecken. Zusätzlich werden einige Bulletpoints für die Marketing-Abteilung abgegeben, so dass diese eine Vorstellung bekommt, was die App künftig leisten wird.
  * **12:45 – 13:40** Michael & Stefan stehen bei Fragen zur Verfügung
  * **13:40 – 13:50** Gruppe 1 – Michael & Stefan geben Feedback
  * **13:50 – 14:00** Gruppe 2 – Michael & Stefan geben Feedback
  * **14:00 – 14:10** Gruppe 3 – Michael & Stefan geben Feedback
  * **14:10 – 14:20** Gruppe 4 – Michael & Stefan geben Feedback
  * **14:20 – 14:30** Gruppe 5 – Michael & Stefan geben Feedback
  * **14:30 – 15:00** Michael & Stefan stehen bei Fragen zur Verfügung
* **15:00 – 16:15** Jede Gruppe präsentiert ca. 8min. Interface von Funktion und User-Journey


## Digital Socializing
Die aktuelle «Corona»-Krise zwingt uns zu neuen Unterrichtsformen wie Home-Schooling. Um das Gefühl einer Klassengemeinschaft zu stärken, möchten wir den heutigen Tag fotografisch dokumentieren. Jede Person macht ein Foto seines Arbeitsplatzes. Zusätzlich wird jede Person einzeln mittels Screenshot via Zoom (möglichst gross) von einem Gruppenmitglied dokumentiert. Die Fotos werden in Slack geposted uns später im Blog-Post verwendet. Wer Privacy-Bedenken hat, wird nicht dazu gezwungen. Als Beispiel machen Michael & Stefan zwischen 8.15 Uhr und 8.45 Uhr den Start.

## Bewertung

### Konzept (30%)
* Funktionen definiert und verständlich
* Das Konzept ist schlüssig und durchgängig
* Informationsarchitektur überlegt
* Zweckmässigkeit gegeben

### Inhalt (10%)
* Inhaltliche Strukturen sind visualisiert
* Funktionen sind vertändlich
* Inhaltselemente sind genügend visualisiert
* Inhalte erscheinen schlüssig

### Interaktion/Führung (50%)
* Interaktion ist schlüssig und schnell zu erlernen
* Kontext in dem sich er User befindet ist verständlich
* Der aktuelle Fortschritt vom Setup ist verständlich
* Die gewählte Funktion vom Tracker ist ersichtlich und editierbar
* Die Userführung ist überlegt und offensichtlich

### Technik (10%)
* Die abgegebene Visualisierung ist für eine technische Realisation aussagekräftig
* Die Realisation mittels App-Technologie ist gegeben







### Vergangene Case Studies
* [IAD2017 · SBB · HS2017](https://signalwerk.github.io/IAD.LAB.DOC/exercise-case-study/) → [Slides](https://signalwerk.github.io/IAD.LAB.SLD/data/2017/KW45-case-study/)
* [IAD2017 · nextpad · FS2018](https://github.com/logrinto/case-study.nextpad)
* [IAD2017 & IAD2019 · Self-Service · HS2019](https://github.com/logrinto/case-study.self-service)
