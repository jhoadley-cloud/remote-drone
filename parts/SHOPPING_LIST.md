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
