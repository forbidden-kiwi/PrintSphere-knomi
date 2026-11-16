# PrintSphere v1.7.6 (Knomi v2)

Adds a GitHub update notice on the Web Config, matching the StatusBar
behavior: a badge next to the version when a newer release exists, plus
Check / Install in the Firmware Update section.

## Changes

- After Wi-Fi and NTP are ready, the device asks GitHub for
  `forbidden-kiwi/PrintSphere-knomi` latest and compares the semver to the
  running firmware.
- If a newer Knomi OTA asset is published, the hero shows **Update vX.Y.Z**.
  Tapping it opens Firmware Update; Install flashes that asset over HTTPS.
- OTA from v1.7.5-knomi_v2 is accepted (same board identity
  `printsphere_knomi_v2_p2`).

## Assets

- `printsphere_full-v1.7.6-knomi_v2.bin` — USB factory flash
- `printsphere_ota-v1.7.6-knomi_v2.bin` — OTA for devices already on the Knomi identity
