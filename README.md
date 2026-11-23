# Gotta Go Fast: engine test cell

A browser jet engine simulator in one file. You design an engine, bolt it to a thrust stand and run it. Everything is unlocked: there are no accounts, paywalls or tracking.

## Play

Open `index.html` in any modern browser. It needs no build step and no server.

## Features

- **Engine types:** turbojet, low- and high-bypass turbofan, turboprop, ramjet and scramjet. Ramjets and scramjets run in a Mach 0–7 wind tunnel.
- **Design office:** set the inlet or fan diameter, pressure ratio, turbine inlet temperature, bypass ratio and propeller diameter. You can also pick the nozzle type, fit an afterburner and choose the hot-section material (steel, nickel superalloy, single-crystal or ceramic matrix).
- **Live design sheet:** shows thrust (kN and lbf), weight, thrust-to-weight, TSFC, airflow, spool-up time, fan pressure ratio and shaft horsepower.
- **Test stand:** run the starter, ignition, fuel and throttle yourself, or use auto start. You can toggle FADEC and the afterburner, change prop pitch gears, and test in standard, tropical (40 °C) or Arctic (−40 °C) conditions.
- **Failures:** compressor surge, flameout, hot starts, and three stages of over-temperature damage that end in a cooked turbine.
- **Dyno:** an automatic test that measures max thrust, best TSFC, spool-up time and afterburner thrust, with a history of your runs.
- **Hangar:** save as many engines as you like (they're stored in your browser), and share designs with build codes.
- **Sound:** engine noise synthesised with the Web Audio API, so there are no audio files.

## Controls

| Key | Action |
|---|---|
| `S` | Auto start / light up |
| `X` | Stop |
| `↑` / `↓` | Throttle |
| `End` | Full power |
| `PgUp` | Afterburner |
| `E` / `Q` | Tunnel speed or prop pitch |

The physics is a simplified Brayton-cycle gas-path model. It aims for believable numbers and is meant for fun, not engineering.
