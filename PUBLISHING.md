# La Familia – Updates veröffentlichen

Dieses öffentliche Repository stellt **nur freigegebene Mod- und Client-Dateien** bereit.

## Mods veröffentlichen
1. Lade eine rechtmäßig weiterverteilbare Forge-1.20.1-Mod unter `updates/files/mods/DATEINAME.jar` hoch.
2. Ermittle lokal ihre SHA-256-Prüfsumme, z. B. in Windows PowerShell:
   `Get-FileHash -Algorithm SHA256 .\\DATEINAME.jar`
3. Ergänze `updates/manifest.json` um `{"path":"mods/DATEINAME.jar","sha256":"ECHTE_64_STELLIGE_PRUEFSUMME"}`.
4. Erhöhe bei Bedarf die Versionsnummer im Manifest und veröffentliche **das Manifest zuletzt**.

Resourcepacks, Shaderpacks und Konfigurationsdateien können analog unter `updates/files/resourcepacks/`, `updates/files/shaderpacks/` und `updates/files/config/` veröffentlicht werden.

Nur Dateien, die im Manifest stehen, werden verteilt. Entfernte Einträge führen dazu, dass der Launcher zuvor von ihm verwaltete Dateien beim nächsten Update entfernt. Andere Dateien werden nicht verändert.

**Wichtig:** GitHub hat Dateigrößenlimits. Für größere Modpacks ist ein Release-Asset- oder CDN-basierter Downloadmechanismus nötig. Lade keine Zugangsdaten oder Dateien ohne Verteilungsrechte hoch.
