# PrintSphere v1.7.9 (Knomi v2)

Fixes chamber-light toggle on H2-series printers.

## Fix

- `ledctrl` now includes the required `led_on_time`, `led_off_time`,
  `loop_times` and `interval_time` fields. H2C/H2D ignored the short payload,
  so the logo went grey for a few seconds and then snapped back while the
  lights stayed on.

## Assets

- `printsphere_full-v1.7.9-knomi_v2.bin` — USB factory flash
- `printsphere_ota-v1.7.9-knomi_v2.bin` — OTA
