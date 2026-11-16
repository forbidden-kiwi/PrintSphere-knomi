# PrintSphere v1.7.5 (Knomi v2)

Merges cptkirki v1.7.5 cloud, config and rendering work into the Knomi port
while keeping the 240×240 layout, CST816 swipe/flick handling and expanded
Latin fonts.

## Release Scope

- **Base**: v1.6.3-knomi_v2 plus upstream v1.7.5.
- **Toolchain target**: ESP-IDF v5.5.4, LVGL v9.5.0.
- **Hardware**: BigTreeTech Knomi v2 (ESP32-S3, GC9A01 240×240, CST816S).
- **Board identity**: `printsphere_knomi_v2_p2` (OTA no longer accepts 1.75 images).

## Taken from upstream v1.7.5

- More reliable Bambu Cloud login, session recovery and printer discovery.
- Command tracking for pause/resume/stop and chamber-light requests.
- Snapshot mailbox so MQTT updates no longer hold the LVGL lock.
- Safer NVS/config store, AMS HT mapping and firmware identity checks.

## Kept from the Knomi port

- Compact 240×240 dashboard, Knomi MDI icon slots and scroll chaining.
- Fast CST816 flicks and finger-down skip of widget rebuilds.
- Latin-1, Euro and Latin Extended-A UI fonts.

## Upgrade

- **USB full flash is required** from v1.6.3: the Knomi image now has its own
  project name, so OTA from `printsphere_1_75_p2` is rejected on purpose.
- Settings written by v1.7.5 may not be readable if you later flash older
  firmware.

## Assets

- `printsphere_full-v1.7.5-knomi_v2.bin` — USB factory flash (bootloader + partitions + app)
- `printsphere_ota-v1.7.5-knomi_v2.bin` — OTA only for devices already on this Knomi identity

## Notes

- Hold BOOT while plugging USB if the serial port does not appear.
- See `NOTICE.md` for upstream attribution.
