# Pflichtenheft

Einführung in das Projekt, Ist- und Sollzustand sind im Projektauftrag ersichtlich.

*1. Schnittstellen*

Der Unity Client ist die zentralle Stelle für die Benutzerinteraktion. 
Der Benutzer nutzt Maus und Tastatur um das Spiel zu steuern.
Wird lokal gespielt, wird die Tastatur und Maus zwischen den Spielern weitergereicht.
Bei einem Online Spiel, kommuniziert der Client im Hintergrund mit einem Go Backend mittels Websockets. 
Das Backend wird in der Google Cloud gehostet.
Die dafür benötigten Daten werden in einer PostgreSQL Datenbank in der Google Cloud gespeichert.
Der Client wird über eine kleine Website zur Verfügung gestellt.

*2. Systemanforderungen*

Der Client soll performant genug laufen, um auf einem Handelsüblichen Notebook gespielt werden zu können. Das Backend soll zumindest 10 Sessions gleichzeitig unterstützen.

*3. Anforderungen für Inbetriebnahme und Einsatz*

Für den Betrieb des Backends wird eine Server Instanz benötigt, die Go code ausführen kann, vorzugsweise ein Linux Container in der Cloud. Als persistenter Speicher soll eine SQL Datenbank dienen. Angedacht hierfür ist eine PostgreSQL Instanz.

*4. Qualitätsanforderungen*

Der Client soll zumindest wie das Spiel eines Indie Developers wirken. Eine Online Spiele Session soll nicht abgebrochen werden, wenn ein Teilnehmer ausfällt. Es soll die Möglichkeit eingebaut werden, auf den Teilnehmer zu warten oder ihn aus dem Spiel entfernen zu lassen, sodass das Spiel fortgesetzt werden kann, wenn noch genügend Spieler vorhanden sind.

*5. Anforderungen an die Projektentwicklung*

Zur Entwicklung werden folgende Tools benötigt: Die Unity Entwicklungsumgebung, ein Go Compiler, ein Code Editor und ein Datenbankmanagement Tool (z.B. DBeaver).
