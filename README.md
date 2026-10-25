# esp32-mesh-framework-gateway

Gateway-Firmware für das **ESP32 Mesh Framework** (Gateway-Hardware: M5Core2, s.
`project.md` §4 im Main-Repo `esp32-mesh-framework`).

**Umfang dieses Repos**

- Gateway-Firmware (Arduino/PlatformIO, ESP-Mesh-Lite als Mesh-Funkstrecke)
- Statischer Web-Server mit UI-Auslieferung von der SD-Card
- WebSocket/JSON-Backend für Browser-UI und Node-RED
- HTTP-Bereitstellung der Knoten-Firmware-Images (Update-Pfad)

**Aktueller Stand (2026-10-25)**

- **Kein Code.** Repo angelegt als leere Hülle, während Phase 0 des Projektplans
  (Prozessfundament) läuft.
- Keine REQ/FSPEC freigegeben, kein Startbefehl erteilt — erste Umsetzungen
  folgen erst nach REQ-Freigabe + FSPEC + explizitem Startbefehl.
- Vorbefüllung erfolgt mit dem ersten autorisierten TASK eines freigegebenen FSPEC.
- Normative Grundlagen finden sich im Main-Repo: `docs/requirements/`,
  `docs/functional_specs/`, `docs/adr/`; Integration erfolgt per `repo@sha`
  gemäß ADR-0003.

**Struktur-Hinweise (geplant, noch nicht angelegt)**

- `src/` Firmware, `data_web/` statische UI-Auslage, `platformio.ini`
- Toolchain-Entscheidungen (ESP-Mesh-Lite-Version, Plattformbindungen) werden
  erst durch die Toolchain-Prüfung (P1.1) und ADR-0001-Freigabe gesetzt.
