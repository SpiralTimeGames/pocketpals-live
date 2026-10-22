# Pocket Pals — live config

`live.json` is downloaded by the Pocket Pals game at startup (and when the app is reopened, at most every
15 minutes) from:

https://raw.githubusercontent.com/SpiralTimeGames/pocketpals-live/main/live.json

Editing this file starts and stops events, switches seasonal animal sets on and off, and changes capsule odds and
shop prices **without an app update**. Changes reach players within about 15–20 minutes.

The full format and step-by-step instructions are in `LIVE_OPS.md` in the private game repository
(SpiralTimeGames/pocketpals).

Rules:
- Keep it valid JSON (a broken file is ignored and players keep the last good one).
- Bump `configVersion` by 1 on every change.
- Dates are UTC.
