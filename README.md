# NET//WORLD · Solo Campaign

Ein spielbarer Browser-Prototyp über das Erkunden eines persistent wirkenden Netzwerks, das Untersuchen von Routern und das Sichern von Spuren. Die Netzwerksimulation ist fiktiv: Das Spiel verbindet sich mit keinen echten Geräten oder Systemen.

## Spielen

Öffne die [Live-Vorschau](https://chaozz2go.github.io/net-world/). Der lokale Spielstand wird automatisch im Browser gespeichert. Ein Neustart löscht diesen Spielstand.

### Kapitel 1 · Signal Lost

1. `ip route` — lokalisiere dein Gateway.
2. Klicke `MA-ACCESS-07` auf der Karte an, verbinde dich und gib `scan` ein.
3. Verbinde dich mit `MA-MAN-02` und scanne dessen Nachbarn.
4. `traceroute RELAY-04` — sichere den fehlerhaften Pfad.
5. `ssh RELAY-04` — reproduziere den abgewiesenen Zugriff.
6. Kehre zu `MA-MAN-02` zurück und gib `show logging` ein.
7. `report` — melde deinen Befund.

### Kapitel 2 · Ghost Route

Verfolge nach dem Abschluss die veraltete Route über `MA-MAN-02`, `FRA-WAN-01` und `EU-BB-01`. Scanne Router, sichere den Traceroute, lies die Backbone-Logs und reiche deinen Bericht ein.

## Befehle

`help`, `ip route`, `connect <gerät>`, `ssh <gerät>`, `disconnect`, `scan`, `ping <ziel>`, `traceroute <ziel>`, `show logging`, `report`, `clear`

Geräte lassen sich auch auf der MAP auswählen. Verbindungen und fehlgeschlagene Zugriffsversuche hinterlassen lokale Spuren, die in den Router-Logs auftauchen. Deine Karte, Missionsfortschritte, XP und Logs bleiben nach einem Reload erhalten.

## Technischer Stand

Statische HTML-/JavaScript-App, ohne Build-Schritt und ohne Server. Die Solo-Kampagne läuft vollständig im Browser. Accounts, ein gemeinsamer Weltzustand, Koop und PvP sind noch nicht implementiert und können später über ein serverseitiges Backend ergänzt werden.
