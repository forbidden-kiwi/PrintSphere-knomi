# PrintSphere v1.7.11 (Knomi v2)

Fixes overlapping main-screen text while local MQTT is still connecting, and restores horizontal page swipe.

## Change

- Handshake copy (`Connecting to local Bambu MQTT`) keeps the layer band; Layer
  and remaining-time stay hidden until the printer link is actually ready.
- Portal IP moves to the remaining-time band during handshake so it cannot
  sit on top of the connecting line.
- Status shows `connecting` instead of leftover `Mqtt`.
- Decorative labels/rows pass horizontal swipe through to the pager. Logo and
  remaining-time taps still work.

## Assets

- `printsphere_full-v1.7.11-knomi_v2.bin` — USB factory flash
- `printsphere_ota-v1.7.11-knomi_v2.bin` — OTA
