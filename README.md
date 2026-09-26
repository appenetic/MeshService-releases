# JUNG HOME Service — Downloads und Updates

Dieses Repository enthält nur die fertigen Pakete von **JUNG HOME Service**, dem Werkzeug
zur Inbetriebnahme und Wartung von JUNG-HOME-Geräten. Der Quellcode liegt woanders.

## Dateien je Release

| Datei | Inhalt |
|---|---|
| `JUNG-HOME-Service-macos.zip` | die App für macOS (Apple Silicon) |
| `JUNG-HOME-Service-windows.zip` | die App für Windows 10/11, 64-bit |
| `update.json` | signierte Beschreibung des Releases; danach sucht die App beim Selbst-Update |
| `hashes.json` | Prüfsummen der Pakete |

## Selbst-Update

Die App prüft beim Start, ob unter
`releases/latest/download/update.json` eine neuere Version steht, zeigt die Änderungen an
und ersetzt sich auf Wunsch selbst. Die Beschreibung ist mit einem Ed25519-Schlüssel
signiert; die App installiert nur, was diese Signatur trägt und dessen Prüfsumme stimmt.

## Lizenz

Die App läuft nur mit einer gültigen, an den Computer gebundenen Lizenzdatei. Anfragen mit
der Computer-ID, die die App anzeigt, an saschaheld@me.com.
