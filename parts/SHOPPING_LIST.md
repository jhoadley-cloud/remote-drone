# Drone Shopping List

This list tracks purchases and unresolved design decisions for the future Pixhawk-based drone.

## Research first

| Priority | Decision | Why it matters | Status |
|---|---|---|---|
| 1 | Airframe type | Quad, hex, fixed-wing, VTOL, etc. changes nearly everything | Not selected |
| 1 | Target all-up weight | Determines motor/prop/ESC/battery sizing | Not selected |
| 1 | Payload | Cameras/sensors/computer affect mass and CG | Not selected |
| 1 | Desired flight time | Drives battery and propulsion sizing | Not selected |
| 1 | Frame size | Sets prop diameter and mounting geometry | Not selected |
| 1 | Manual/autonomous mission | Determines radio, GPS, telemetry, sensing | Not selected |

## Likely purchases for a multirotor path

| Item | Qty | Requirement | Budget | Status | Notes |
|---|---:|---|---:|---|---|
| Airframe/frame | 1 | Size TBD after mission definition | TBD | Researching | Could be purchased or printed/prototyped |
| Brushless motors | 4+ | Matched set sized to prop + weight | TBD | Researching | Count depends on frame |
| ESCs | 4+ or integrated | Matched to motor current + battery | TBD | Researching | Owned Aero Selfie boards are driver/distribution boards, not assumed to be ESCs |
| Propellers | Multiple sets | Matched to motors/frame | TBD | Researching | Buy spares |
| Prop adapters/hardware | Set | Match motors/props | TBD | Researching | |
| Power distribution | 1 | Rated for total current | TBD | Researching | May be integrated depending architecture |
| Flight-controller power module | 1 | Pixhawk-compatible, voltage/current appropriate | TBD | Researching | Inspect owned Pixhawk bundle first |
| GPS + compass | 1 | ArduPilot compatible | TBD | Researching | Inspect owned Pixhawk bundle first |
| RC transmitter | 1 | Enough channels for modes/arm/failsafe | TBD | Researching | May be shared with rover if suitable |
| RC receiver | 1 | Pixhawk-compatible | TBD | Researching | |
| Telemetry radio | 1 set | MAVLink compatible | TBD | Optional | |
| Battery charger | 1 | Must safely support selected cell count/capacity | TBD | Researching | Confirm current charger inventory first |
| LiPo-safe storage | 1 | Storage/transport | TBD | Researching | |
| Landing gear | 1 set | Frame/payload dependent | TBD | Researching | Can be 3D printed |
| Vibration isolation | 1 set | Flight controller mounting | TBD | Researching | |
| Wiring/connectors | Assorted | Sized for current | TBD | Researching | Some already owned |
| Fasteners/standoffs | Assorted | Frame-specific | TBD | Researching | |

## Do not purchase yet

Do not buy motors, propellers, ESCs, a frame, or another flight battery until the mission, aircraft type, target weight, and propulsion architecture are defined.


## OpenDrone quadcopter procurement plan (2026-10-18)

**Selected:** [ljbotero/OpenDrone printable frame](https://github.com/ljbotero/OpenDrone), a Pixhawk-oriented quadcopter. The designer's [original tested configuration](https://github-wiki-see.page/m/ljbotero/OpenDrone/wiki/Configurations-%26-Parts) used 4 x DYS D4215 650KV motors, 4 x 40A 2–6S ESCs, 12x3.8 props, F450/F550 arms and a 6S pack. This is a historical reference, **not** a validated bill of materials for our exact print and battery.

**Already owned:** Pixhawk 2.4.8 bundle (verify power module/GPS/safety switch/buzzer), Spektrum 6S 3200mAh battery, BETAFPV Cetus Pro FPV Kit (LiteRadio 2 SE FrSky D8 controller + VR02 5.8GHz analog goggles), tools and printer, one unverified 60A ESC, two Aero Selfie interface boards. Do not repurchase until checked.

**Amazon links below are Amazon SEARCH links, not verified in-stock product listings.** No prices or exact seller claims are implied. Before ordering, confirm electrical ratings, connectors, mechanical dimensions, and frame/prop clearances.

| Priority | Purchase / search | Qty | Amazon search | Status / acceptance criteria |
|---|---|---:|---|---|
| 1 | **FrSky D8-compatible receiver with SBUS output** (e.g. genuine/verified FrSky D8-capable receiver) | 1 | [Amazon: FrSky D8 SBUS receiver](https://www.amazon.com/s?k=FrSky+D8+SBUS+receiver) | **Required to reuse LiteRadio 2 SE.** Verify **D8**, not merely D16/ACCESS/ELRS, and SBUS/PPM output. Verify failsafe behavior and bind before flight. |
| 1 | Pixhawk RC IN / SBUS receiver cable | 1 | [Amazon: Pixhawk SBUS receiver cable](https://www.amazon.com/s?k=Pixhawk+2.4.8+SBUS+receiver+cable) | Required unless supplied with Pixhawk/receiver. Check connector pinout and receiver supply voltage. |
| 1 | 6S-rated 650KV-class multirotor motors, D4215-class | 4 | [Amazon: D4215 650KV drone motor](https://www.amazon.com/s?k=D4215+650KV+drone+motor) | **Hold for thrust calculations**; match 6S, prop size, motor mount pattern, and airframe. |
| 1 | 40A-class 6S brushless multirotor ESCs | 4 total | [Amazon: 40A 6S multirotor ESC](https://www.amazon.com/s?k=40A+6S+multirotor+ESC) | May count owned 60A ESC **only after** checking firmware, current rating, PWM control and compatibility. Prefer four matching ESCs. |
| 1 | 12x3.8 propeller pairs CW/CCW | 2 pairs + spares | [Amazon: 12x3.8 quadcopter props](https://www.amazon.com/s?k=12x3.8+quadcopter+propellers+CW+CCW) | **Hold** until motor thrust data, clearance, shaft/hub and correct rotation confirmed. |
| 1 | F450/F550 compatible frame arms (if required by original CAD) | 4 | [Amazon: F450 replacement arms](https://www.amazon.com/s?k=F450+quadcopter+replacement+arms) | Inspect STL assembly; original reference uses arms in addition to printed body. |
| 1 | 6S-capable power distribution board / harness | 1 | [Amazon: 6S quadcopter power distribution board](https://www.amazon.com/s?k=6S+quadcopter+power+distribution+board) | Rated for combined ESC current; inspect owned boards first. |
| 1 | Pixhawk 2.4.8-compatible **6S-rated** power module | 1 | [Amazon: Pixhawk 2.4.8 6S power module](https://www.amazon.com/s?k=Pixhawk+2.4.8+6S+power+module) | Check voltage/current limits and 6-pin connector pinout; **not all old 3DR modules safely support fully charged 6S (25.2V)**. Inspect bundle first. |
| 1 | GPS/compass module with mast | 1 | [Amazon: Pixhawk GPS compass M8N](https://www.amazon.com/s?k=Pixhawk+2.4.8+M8N+GPS+compass) | Only if missing from owned bundle. Check wiring and compass compatibility. |
| 1 | Pixhawk safety switch and buzzer | 1 each | [Amazon: Pixhawk 2.4.8 safety switch buzzer](https://www.amazon.com/s?k=Pixhawk+2.4.8+safety+switch+buzzer) | Only if missing from bundle. |
| 2 | **5.8GHz analog FPV camera** | 1 | [Amazon: analog FPV camera](https://www.amazon.com/s?k=5.8GHz+analog+FPV+camera+NTSC+PAL) | Compatible composite analog video output for VTX; don't confuse with digital-only camera. |
| 2 | **5.8GHz analog FPV VTX**, antenna included | 1 | [Amazon: 5.8GHz analog FPV VTX](https://www.amazon.com/s?k=5.8GHz+analog+FPV+video+transmitter+antenna) | Required to use **owned BETAFPV VR02 goggles**; match supported channels and power input. Never power VTX without antenna if manufacturer prohibits it. |
| 2 | Regulated 5V/9V BEC for camera/VTX (as needed) | 1 | [Amazon: 6S to 5V 9V BEC](https://www.amazon.com/s?k=6S+to+5V+9V+BEC+drone) | Only after selecting camera/VTX; check voltage and current requirements. |
| 2 | Pixhawk anti-vibration mounting pads/platform | 1 | [Amazon: Pixhawk vibration mount](https://www.amazon.com/s?k=Pixhawk+vibration+damping+mount) | Verify dimensions and clearance. |
| 2 | Battery straps, hook-and-loop, anti-slip pad | 1 set | [Amazon: drone battery straps](https://www.amazon.com/s?k=drone+LiPo+battery+straps) | Secure owned 6S pack and verify CG. |
| 2 | XT60/XT90 connectors, silicone wire, heat-shrink | Assorted | [Amazon: drone XT60 wire kit](https://www.amazon.com/s?k=XT60+silicone+wire+heat+shrink+kit) | Match **actual** battery connector and worst-case current; check owned stock first. |
| 2 | Metric bolts, locknuts, standoffs | Assorted | [Amazon: M2.5 M3 drone screw kit](https://www.amazon.com/s?k=M2.5+M3+drone+standoff+screw+kit) | Match STL and motor mount drawings; no assumed screw length. |
| 2 | 6S LiPo balance charger | 1 | [Amazon: 6S LiPo balance charger](https://www.amazon.com/s?k=6S+LiPo+balance+charger) | Only if not owned. Must support pack connector, chemistry and balance lead. |
| 2 | LiPo fire-resistant storage bag / safe storage solution | 1 | [Amazon: LiPo safe storage bag](https://www.amazon.com/s?k=LiPo+fire+resistant+storage+bag) | Supplemental containment, not a guarantee against fire. |
| 3 | MAVLink telemetry radio pair | 1 pair | [Amazon: Pixhawk telemetry radio](https://www.amazon.com/s?k=Pixhawk+MAVLink+telemetry+radio+pair) | Optional, but useful for Mission Planner/QGroundControl; choose legal local frequency. |
| 3 | Landing gear and GPS mast hardware | As needed | [Amazon: F450 landing gear](https://www.amazon.com/s?k=F450+quadcopter+landing+gear) | Print if practical; check frame STL. |

### LiteRadio 2 SE -> Pixhawk 2.4.8: required integration

`LiteRadio 2 SE (FrSky D8 2.4GHz)` -> **D8-compatible receiver** -> `SBUS or PPM output` -> **Pixhawk RC IN** -> ArduPilot radio calibration, mode switches and verified loss-of-signal failsafe.

- The transmitter **cannot bind directly to the Pixhawk**; the receiver and correctly pinned RC cable are essential.
- Confirm receiver supports **FrSky D8**, not just a vaguely advertised “FrSky compatible” protocol. Some regional/firmware revisions differ.
- Select a receiver with SBUS or PPM output. Standard individual PWM channel pins alone will need an additional PPM encoder.
- Bench-test binding, channel mapping, switches, throttle range and failsafe **with propellers removed**. Confirm sufficient independent channels for arming and flight modes. Check receiver voltage and SBUS inversion support.
- Do **not** buy an ELRS-only receiver for this transmitter. If reliable D8/SBUS hardware cannot be sourced, reconsider the radio architecture before buying motors.
- The VR02 goggles receive **5.8GHz analog video** from a separate analog camera + VTX on the drone; they do not receive video from the Pixhawk or Raspberry Pi automatically.

### Purchase gates (must resolve before buying propulsion)

1. Weigh the printed frame, arms, payload and installed battery; set target all-up weight and desired flight time.
2. Verify 12-inch propeller clearance and structural suitability of the actual STL/arm configuration.
3. Obtain motor manufacturer thrust/current data for the exact 6S + prop combination; target adequate thrust margin.
4. Check actual Spektrum pack connector, continuous discharge rating, size and condition.
5. Inventory the Pixhawk kit (power module, GPS/compass, cables, buzzer, switch), owned ESC and charger.
6. Do radio receiver binding/failsafe bench test and inspect frame before flight. Printed PLA frame suitability must be evaluated rather than assumed.

Sources: [BETAFPV Cetus Pro specifications](https://betafpv.com/products/cetus-pro-fpv-kit), [ArduPilot receiver connections](https://ardupilot.org/copter/docs/common-rc-systems.html), [OpenDrone original configuration](https://github-wiki-see.page/m/ljbotero/OpenDrone/wiki/Configurations-%26-Parts).
