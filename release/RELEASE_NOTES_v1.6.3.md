# PrintSphere v1.6.3 (Knomi v2)

Patch release on top of v1.6.2 for German umlauts and other Latin characters
on the display. OTA-compatible with v1.6.2 Knomi images (no partition table
change).

## Release Scope

- **Base**: v1.6.2-knomi_v2.
- **Toolchain target**: ESP-IDF v5.5.4, LVGL v9.5.0.
- **Hardware**: BigTreeTech Knomi v2 (ESP32-S3, GC9A01 240×240, CST816S).

## Fixes

- **German umlauts render on the Knomi UI**: The compact Montserrat 12/14
  fonts used on Knomi v2 now include `Ä Ö Ü ß ä ö ü` plus printable ASCII
  and the degree sign, so job names and printer names no longer show tofu.
- **UTF-8 strings stay intact**: Truncating job names, status labels and
  short display names no longer splits a multi-byte character in the middle.

## Assets

- `printsphere_full-v1.6.3-knomi_v2.bin` — USB factory flash (bootloader + partitions + app)
- `printsphere_ota-v1.6.3-knomi_v2.bin` — OTA only for devices already on Knomi v2

## Notes

- Hold BOOT while plugging USB if the serial port does not appear.
- See `NOTICE.md` for upstream attribution.
