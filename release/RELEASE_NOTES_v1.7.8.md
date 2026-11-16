# PrintSphere v1.7.8 (Knomi v2)

Fixes GitHub Install / Reinstall OTA failing with `ESP_FAIL`.

## Fix

- GitHub release assets redirect to a long signed CDN URL. The HTTP client
  now uses a 4 KB buffer, sends a User-Agent, follows those redirects first,
  then flashes the final HTTPS URL.

## Assets

- `printsphere_full-v1.7.8-knomi_v2.bin` — USB factory flash
- `printsphere_ota-v1.7.8-knomi_v2.bin` — OTA (file upload or USB; GitHub
  install on v1.7.7 may still fail until this build is on the device)
