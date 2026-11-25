# Mesh Service – Downloads und Updates

Dieses Repository enthält die fertigen Pakete von **Mesh Service**, der Software für die
Inbetriebnahme, Einstellung und Analyse von Bluetooth-Mesh-Anlagen. Unterstützt werden Geräte von
JUNG HOME und Steinel. Der Quellcode liegt nicht hier.

Website: https://meshservice.de/

## Dateien je Release

| Datei | Inhalt |
|---|---|
| `Mesh-Service-macos.zip` | das Programm für macOS 14 oder neuer, Mac mit Apple-Chip |
| `Mesh-Service-windows.zip` | das Programm für Windows 10 (ab 1709) und Windows 11, 64 Bit |
| `Mesh-Service-Anleitung-X.Y.Z.pdf` | die Anleitung auf Deutsch |
| `Mesh-Service-Manual-X.Y.Z.pdf` | die Anleitung auf Englisch |
| `update.json` | signierte Beschreibung des Releases; danach sucht das Programm beim Update |
| `hashes.json` | Prüfsummen der Pakete |

Die neueste Version laden Sie direkt über
`releases/latest/download/Mesh-Service-macos.zip` bzw. `…/Mesh-Service-windows.zip`.

## Updates

Das Programm prüft beim Start und alle sechs Stunden, ob unter
`releases/latest/download/update.json` eine neuere Version steht, zeigt die Änderungen an und
ersetzt sich auf Wunsch selbst. Die Beschreibung ist mit einem Ed25519-Schlüssel signiert; das
Programm installiert nur Pakete mit gültiger Signatur und passender Prüfsumme.

## Lizenz

Das Programm läuft nur mit einer gültigen Lizenzdatei, die an den Rechner gebunden ist. Die
Anfrage mit der Computer-ID, die das Programm anzeigt, geht an saschaheld@me.com.
