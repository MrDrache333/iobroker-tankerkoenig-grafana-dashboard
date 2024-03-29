# iobroker-tankerkoenig-grafana-dashboard

Dieses Dashboard visualisiert Daten des Tankerkönig Adapters für [ioBroker](https://iobroker.net/) mit einer InfluxDB Datenbank als Datenquelle.

![](dashboard.jpg)

## Vorraussetzungen

- Grafana 6.7.3 oder höher
- InfluxDB Datenbank (<2.0)
- Tankerkönig Adapter konfiguriert und laufend in ioBroker
- InfluxDB-Adapter konfiguriert und laufend in ioBroker
  - Das Dashboard benötigt für jede hinzugefügte Tankstelle den Preis (short), den Namen und den "geöffnet" Status (status). Der Preis hängt von der gewählten Kraftstoffart ab und sollte ebenfalls erfasst werden, um eine korrekte Darstellung im Dashboard zu ermöglichen.

## Installation

1. Lade die `dashboard.json` Datei von diesem Repository herunter.
2. In Grafana gehe zur Dashboard-Liste und klicke auf den "Importieren" Button in der oberen rechten Ecke.
3. Wähle die Option "Upload .json Datei" aus und wähle die heruntergeladene `dashboard.json` Datei aus.
4. Wähle die InfluxDB Datenquelle aus dem Dropdown-Menü aus.
5. Klicke auf den "Importieren" Button, um den Import des Dashboards abzuschließen.

## Verwendung

Das Dashboard sollte nun in der Dashboard-Liste verfügbar sein und kann durch Klicken auf den Namen geöffnet werden.

Das Dashboard enthält Panels, die verschiedene Aspekte der Daten vom Tankerkönig Adapter visualisieren, wie zum Beispiel die Preise verschiedener Treibstofftypen an verschiedenen Tankstellen. Verwende den Zeitbereich-Selector und den Aktualisieren Button in der oberen rechten Ecke, um die angezeigten Daten zu steuern. Außerdem lässt sich oben links über das Auswahlfeld "Kraftstoff" die Kraftstoffart auswählen. Zur Auswahl stehen e5, e10 und Diesel
