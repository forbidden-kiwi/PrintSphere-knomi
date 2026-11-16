# PrintSphere v1.7.10 (Knomi v2)

Enables logo-tap light control on A1-family printers.

## Change

- A1, A1 Mini, P1P and A2L report MQTT node `chamber_light` for the
  toolhead/logo LED. The capability table had that flag off, so the logo
  was not clickable even though the same `ledctrl` command works.

## Assets

- `printsphere_full-v1.7.10-knomi_v2.bin` — USB factory flash
- `printsphere_ota-v1.7.10-knomi_v2.bin` — OTA
