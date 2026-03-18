# Shellycone

**Shellycone** stellt eine Sammlung von Loxone-Addons für Shelly-Geräte bereit.
Die Addons können einfach über die Loxone Config als virtuelle HTTP-Ein- und Ausgänge importiert werden.

## Features

* Einfache Integration von Shelly-Geräten in Loxone
* Auslesen von Messwerten (z. B. Leistung, Spannung, Strom, Energie)
* Schalten von Relais über HTTP im lokalen Netzwerk
* Nutzung bestehender Shelly RPC- und REST-APIs
* Schneller Import per XML in die Loxone Config

## Voraussetzungen

* Loxone Miniserver
* Loxone Config
* Shelly-Gerät (z. B. Shelly Plug S)
* Netzwerkzugriff auf das Gerät
* IP-Adresse des Gerätes ist bekannt

## Installation

1. XML-Datei aus diesem Repository herunterladen
2. In der Loxone Config:
   * Virtuellen HTTP Eingang/Ausgang auswählen
   * XML importieren
3. IP-Adresse des Shelly-Geräts in den Einstellungen des Eingangs/Ausgangs anpassen
4. Konfiguration in den Miniserver laden

## Nutzung

Nach dem Import stehen folgende Ein- und Ausgänge zur Verfügung:

Eingänge:
- Relais_0 (Schaltzustand)
- Power (Leistung in kW)
- Voltage (Spannung in V)
- Current (Strom in A)
- Energy_total (Gesamtenergie in kWh)
- Energy_by_minute_0 (Energie pro Minute in Wh)
- Energy_minute_ts (Zeitstempel der Energiedaten)
- Temperatur_C (Temperatur in °C)
- Temperatur_F (Temperatur in °F)

Ausgänge:
- Relais (An/Aus)

Diese können direkt in Visualisierung, Logikbausteinen oder Automationen verwendet werden.

## Ziel

Ziel dieses Projekts ist es, die Integration von Shelly-Geräten in Loxone möglichst einfach, flexibel und transparent zu gestalten – ohne zusätzliche Middleware oder Cloud-Abhängigkeiten.

## Dateien
[Geräte]("Shellys")

## Lizenz

MIT License
