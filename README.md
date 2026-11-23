# Gotta Go Fast: engine test cell

A browser jet engine simulator in one file. You design an engine, bolt it to the stand in a gritty concrete test cell and run it. Everything is unlocked: there are no accounts, paywalls or tracking.

## Play

Open `index.html` in any modern browser. It needs no build step and no server.

## Features

### Test cell
- A live cutaway of the engine on its thrust stand. The fan, compressor and turbine blades actually spin, the combustor glows with turbine temperature, and the plume roars into the exhaust collector.
- The bay has floodlights, hazard stripes and an intake danger zone. The afterburner glow lights up the room, and the cell shakes when something goes wrong.
- A console with analogue dials (N1, N2, turbine temperature, fuel flow, thrust, vibration), warning lights, a green-screen readout, a thrust trace and a throttle lever.

### Engines and parts
- **Types:** turbojet, turbofan, turboprop, ramjet and scramjet.
- **Design settings:** fan or inlet size, pressure ratio, turbine temperature, bypass ratio and propeller size.
- **Cooling air** lets the turbine run hotter than the material limit, at a cost in efficiency.
- **Customer bleed air** costs thrust.
- **Spools:** single or twin. Twin spool gives more surge margin.
- **Variable inlet guide vanes** improve stall margin.
- **Thrust reverser.**
- **Inlet:** fixed pitot, or a variable ramp for supersonic flight.
- **Nozzle:** convergent or convergent–divergent.
- **Afterburner.**
- **Materials:** steel, nickel superalloy, single-crystal or ceramic matrix.
- Every design has a weight, a build cost and a surge margin.

### Flight envelope
- An ISA atmosphere from 0 to 30 km and Mach 0 to 8, plus hot and Arctic days.
- Inlet shock losses and ram drag. Compressor exit temperature limits the engine at high Mach.
- Windmill airstarts, and flameouts when the air gets too thin to burn.
- A thrust map across altitude and Mach. Click anywhere on it to test at that condition.

### Contracts
Thirteen contracts, from a flight school trainer and a topdressing plane to an interceptor, a ramjet missile and a hypersonic demonstrator. Each one has requirements on thrust, fuel burn, weight, cost, spool-up time, shaft power, bleed air or a reverser. Run certification and the cell flies the test for you, then grades it from 1 to 3 stars.

### Sound
The engine sound is synthesised from the noise sources real engines make:
- jet mixing roar, pitched by jet speed and nozzle size
- fan and compressor blade-passing tones
- buzz-saw tones when big fan tips go supersonic
- combustion rumble
- afterburner roar with crackle
- the air starter whine and ignitor ticks
- the light-off "whoomp" and the surge bang
- the turboprop's blade-pass drone

Everything plays through a concrete-room reverb.

### Also
- Failures: compressor surge, hot starts, flameout, and turbine or compressor over-temperature damage that ends in a destroyed engine.
- An automatic dyno test, unlimited saved engines and shareable build codes.

## Controls

| Key | Action |
|---|---|
| `S` | Auto start / light up |
| `X` | Shutdown |
| `↑` / `↓` | Throttle |
| `End` | Full power |
| `PgUp` | Afterburner |
| `R` | Reverser |
| `E` / `Q` | Mach up / down |
| `W` / `A` | Altitude up / down |
| `[` / `]` | Prop pitch |

The physics is a simplified gas-path model. It aims for believable numbers and is meant for fun, not engineering.
