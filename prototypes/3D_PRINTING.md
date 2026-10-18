# Drone 3D Printing Prototype Index

Track downloadable reference models and custom CAD for the drone project here.

## Reference candidates

| Candidate | What it helps with | Fit status | Source |
|---|---|---|---|
| AX540 hexacopter frame | Full printable large hexacopter reference | Possible future architecture; separate sizing analysis required | https://www.printables.com/model/1165926-ax540-hexacopter-frame |
| FlyFishRC VX3.5 GPS mount | GPS mount with STL/F3Z/STEP files | Frame-specific; useful CAD reference | https://www.printables.com/model/1067241-flyfishrc-vx35-gps/files |
| Volador VX5 GPS mount for 21x21 mm modules | TPU GPS mounting concept | Frame-specific; useful if GPS is 21x21 mm | https://www.printables.com/model/877265-volador-vx5-t700-gps-mount-hglrc-m100-5883-and-oth |
| SpeedyBee Master 5 V2 GPS/compass mount | Level GPS/compass mounting concept | Frame + GPS specific | https://www.printables.com/model/1485002-speedybee-maser-5-v2-mateksys-m10q-5883-gps-compas |
| TBS Source One V5 receiver tray | Small receiver tray mounting concept | Frame-specific | https://www.printables.com/model/315216-rc-rx-mounting-tray-tbs-source-one-v5 |

## Custom CAD queue

| Prototype | Inputs needed | Goal | Status |
|---|---|---|---|
| Pixhawk vibration mount | Frame stack dimensions, Pixhawk footprint | Isolate FC while retaining access | Waiting on frame |
| GPS/compass mast | GPS dimensions + frame geometry | Level module away from high-current wiring | Waiting on frame/GPS |
| Receiver/telemetry tray | Radio modules + frame | Organized low-mass mounting | Waiting on electronics |
| Camera mount | Camera choice + desired angle | Protected adjustable camera | Optional |
| Raspberry Pi mount | Pi use case + payload allowance | Rigid, cooled companion-computer mount | Optional |
| Landing gear | Prop/frame clearance + payload | Stable takeoff/landing and sensor clearance | Waiting on frame |
| Fog-flow test fixture | Motor/prop geometry | Safe bench fixture for smoke-flow visualization | Researching |

## Prototype sequence

1. Select airframe architecture.
2. Define target weight, payload, and flight-time goal.
3. Select frame size and propulsion system.
4. Measure the Pixhawk and chosen GPS/receiver/telemetry modules.
5. CAD low-risk mounts first.
6. Print inexpensive fit-check prototypes.
7. Validate clearances, cable routing, vibration isolation, and CG.
8. Reprint flight-ready parts in an appropriate material.
