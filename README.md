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
- **Types:** turbojet, turbofan, turboprop, helicopter turboshaft, ramjet and scramjet.
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

### Design office
A step-by-step build across 13 sheets. Each sheet has a live cutaway with that part highlighted, a diagram of its own, and a data plate:
- **Identity:** name, notes, presets, the hangar and build codes.
- **Layout:** engine type, inlet size and inlet type.
- **Compressor:** stages, pressure ratio, efficiency, bleed and guide vanes.
- **Fan or prop:** bypass ratio, plus fan pressure ratio (set it yourself or let it auto-match).
- **Combustor:** turbine temperature, pressure loss and cooling.
- **Turbine:** material, stages and efficiency.
- **Nozzle:** shape, throat area and reverser.
- **Afterburner:** fuel rate and nozzle opening, with a check for choking and liner burn-through.
- **Rotor:** single, twin or triple spool, disc material (sets the speed limit) and rotor mass.
- **FADEC:** fitted or not, idle speed, and a throttle map you drag into shape.
- **Conditions.**
- **Airframe:**
  - Wing: area, sweep (from 45° forward to 70° back), aspect ratio, taper (down to a pure delta) and position along the body.
  - Tail: conventional tail, canards, canards plus tail, or tailless delta, with tail area and sweep.
  - Fins: single or twin, with fin area and cant angle.
  - Fuselage, fuel, structure (forward sweep needs carbon composite) and single or twin engines.
  - Checks for engine fit plus pitch, yaw and wing-twist stability, then mass, drag polar and performance figures.
  - Frame presets in F-22, F-35, Mirage and Su-47 style.
  - An animated flight test: take-off roll, climb to 11 km, top speed and range. An unstable design departs instead.
- **Review:** a list of design problems.

### Helicopter turboshaft
The turboshaft drives a water-brake dyno. The governor holds the rotor at 100% while you raise the collective. Turn the governor off and you have to stop the rotor overspeeding yourself.

### Goals and records
- 13 goals with ranks, from first light to hypersonic.
- Records kept on this device: most thrust, best thrust/weight, lowest fuel burn, quickest spool-up, most shaft power and fastest flight test.

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
| `↑` / `↓` | Throttle ±5% (hold Shift for ±1%) |
| `Home` / `End` | Idle / full power |
| `End` | Full power |
| `PgUp` | Afterburner (or push the throttle past the 100% gate) |
| `R` | Reverser |
| `E` / `Q` | Mach up / down |
| `W` / `A` | Altitude up / down |
| `[` / `]` | Prop pitch or collective |
| `T` | Thermal view |

The physics is a simplified gas-path model. It aims for believable numbers and is meant for fun, not engineering.
