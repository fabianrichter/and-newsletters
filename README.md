# AND Newsletter Repository

## Setup

Als erstes muss (falls nicht schon vorhanden), Nodejs und NPM installiert werden.
Anschließend wird einmalig `npm install` ausgeführt, um die Abhängigkeiten zu installieren.


## Entwicklung

### MJML

[MJML (Mailjet Markup Language)](https://mjml.io/) ist eine Sprache zum Entwicklung von HTML-Emails in spezieller XML-Syntax. Es erweitert die Kompatibilität auf alte Mail-Clients und stellt sicher, dass responsive Emails auf allen Email-Clients gut angezeigt wird, ohne selbst komplexe HTML3-Tabellen zu nutzen. Durch das Verwenden von MJML wird die Entwicklung von Emails und Email-Templates stark erleichtert.  

→ [Hier gehts zur Dokumentation von MJML](https://documentation.mjml.io/)  
→ [Hier gehts zum online Editor von MJML](https://mjml.io/try-it-live)

### Anwendung

MJML-Kommandos werden mit `npx mjml` ausgeführt.

**Beispiele und häufig verwendete Kommandos**

| Beschreibung | Kommando |
| --- | --- |
| Auflisten aller Kommandos | `npx mjml --help` |
| Kompilieren einer MJML-Datei | `npx mjml -r <input>.mjml -o <output>.html`
| Starten eines MJML Watch-Servers zum Kompilieren bei Änderungen | `npx mjml -r <input>.html -o <output>.html -w` |


### Weitere Informationen

Bei Nutzung von VS-Code kann auch die MJML-Erweiterung installiert werden. Damit kann das MJML in einer Preview ausgegeben werden, welche auf Live-Änderungen reagiert. Außerdem kann das HTML direkt aus der MJML-Datei kopiert und exportiert werden.

Die Newsletterdateien der verangenen Veranstaltungen sind im Ordner `./newsletter` abgelegt. Es sollte immer die neueste Version eines Newsletters kopiert und angepasst werden, sowie in dem entsprechenden Jahresordner angelegt werden.