# GeoFS Smart HUD

A clean, glass-cockpit style heads-up display for [GeoFS](https://www.geo-fs.com/), delivered as a Tampermonkey userscript.

![status](https://img.shields.io/badge/version-1.0.0-7fffd4) ![type](https://img.shields.io/badge/type-Tampermonkey%20userscript-blue) ![compatible](https://img.shields.io/badge/GeoFS-v3.9%20%7C%20v4.0-orange)        
data:image/png;base64,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


Compatible with GeoFS **v3.9** and **v4.0**.

## Features

- **Ground Speed** — computed live from the aircraft's position over a rolling ~2 second window (GeoFS doesn't expose a raw ground speed value, so this is calculated using great-circle distance / time, smoothed to avoid jitter)
- **Indicated Airspeed (IAS)** — knots
- **True Airspeed (TAS)** — knots
- **Altitude** — feet (MSL)
- **Vertical Speed** — feet per minute
- Draggable, position persists between sessions
- Toggle visibility anytime with **Shift + X**
- Dark glass panel styling with cyan/amber PFD-style readouts — built to look like it belongs in the cockpit, not bolted onto the browser

## Installation

1. Install the [Tampermonkey](https://www.tampermonkey.net/) browser extension if you don't already have it.
2. Open the [raw script file](https://raw.githubusercontent.com/eudes0144-commits/Geofs-Smart-HUD/main/geofs-smart-hud.user.js) — Tampermonkey should prompt you to install it directly.
3. Confirm the install, then head to [geo-fs.com](https://www.geo-fs.com/) and load into a flight.
4. The HUD appears top-right once the aircraft finishes loading.

Because this script includes `@updateURL`/`@downloadURL` pointing at this repo, Tampermonkey will automatically check for and offer newer versions — no manual reinstall needed for future updates.

## Usage

| Action | How |
|---|---|
| Show/hide HUD | `Shift + X` |
| Move HUD | Drag the header bar |
| Close HUD | Click the ✕ in the header |

## How it reads the game

GeoFS doesn't publish official documentation for its internals, so this script pulls values from properties recovered through GeoFS's public TypeScript typings (`@geps/geofs-types`) and cross-referenced against community userscripts:

| Readout | Source |
|---|---|
| IAS | `geofs.animation.values.kias` |
| TAS | `geofs.animation.values.ktas` (falls back to `.tas`) |
| Altitude | `geofs.animation.values.altitude` |
| Vertical Speed | `geofs.animation.values.climbrate` (falls back to `.verticalSpeed`) |
| Ground Speed | Not exposed by GeoFS — calculated in-script from `geofs.aircraft.instance.llaLocation` position deltas |

If GeoFS changes these internal property names in a future update, the affected readout will show `--`. Check the browser console for `[Smart HUD]` log lines — the script logs its startup state to make debugging that easy.

## Known limitations

- No flight-plan / ETA tracking. This was attempted in an earlier version but GeoFS's native flight-plan feature isn't exposed as a stable, scriptable object, and manual waypoint entry (typing lat/long for every point) wasn't worth the friction. May revisit if a reliable read path is found.
- Ground speed is a live estimate, not a raw sim value — expect a brief settling period right after a sudden speed change.

## Roadmap / ideas

- [ ] Flight-plan read + ETA/TOD tracking, if a stable data source is found
- [ ] Wind-corrected GS/TAS delta readout
- [ ] OAT / autopilot altitude & heading bug display

## Contributing

This is a personal project — issues and suggestions welcome via GitHub Issues on this repo.

## Credits

- **[eudes0144-commits](https://github.com/eudes0144-commits)** — creator and maintainer
- Built with the help of **Claude** (Anthropic)
- Field/property references pulled from GeoFS's public [`@geps/geofs-types`](https://gpsystem.github.io/geofs-types/) typings, and cross-checked against community userscripts including the [GeoFS GPWS Alerts](https://greasyfork.org/en/scripts/523621-geofs-gpws-alerts) script by Avramator
- Thanks to the wider GeoFS modding community for documenting the sim's internals despite it having no official public API

## License

MIT — do whatever you want with it.
