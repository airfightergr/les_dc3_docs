# Controls Setup

Our DC-3 has a lot of customized systems, and we **highly recommend** to create a unique controls profile.
We have implement some of the standard (default) commands, where it was possible, but also added custom commands, to allow proper control of the aircraft.

The list below contains those commands that are essential. This document will be updated in the future, with any changes or additions.

**DESCRIPTION:** What you should search for in X-Plane settings.<br>
**COMMAND:** The actual command.
____
#### LANDING GEAR 
Lowers or raises the landing gear. Levers in the cockpit as set at their respective positions.

| DESCRIPTION                                  | COMMAND                                       |
|----------------------------------------------|-----------------------------------------------|
| Landing gear toggle                          | sim/flight_controls/landing_gear_toggle       |

____
#### FLAPS
Hold continuously to achieve the required flaps' position.

| DESCRIPTION        | COMMAND                        |
|--------------------|--------------------------------|
| Flaps up a notch   | sim/flight_controls/flaps_up   |
| Flaps down a notch | sim/flight_controls/flaps_down |

____
#### PARKING BRAKES
Toggles parking brakes.

| DESCRIPTION              | COMMAND                               |
|--------------------------|---------------------------------------|
| Toggle brakes max effort | sim/flight_controls/brakes_toggle_max |

____
#### TAIL WHEEL LOCK
Unlocks or locks the tail wheel. Keep in mind, if you lock the tail wheel, and it is not aligned with aircraft's longitudinal axis, will not be lock until be aligned.

| DESCRIPTION      | COMMAND                   |
|------------------|---------------------------|
| Tail Wheel Lock  | les/dc3/controls/tailLock |

____

#### PITCH TRIM
Pitch trim is mechanical, so you must select the proper command.

| DESCRIPTION                             | COMMAND                                  |
|-----------------------------------------|------------------------------------------|
| Pitch trim up - Mechanical, not servo   | sim/flight_controls/pitch_trim_up_mech   |
| Pitch trim down - Mechanical, not servo | sim/flight_controls/pitch_trim_down_mech |

____

#### TRIMS
Pitch trim is mechanical, so you must select the proper command.

| DESCRIPTION                             | COMMAND                                  |
|-----------------------------------------|------------------------------------------|
| Pitch trim up - Mechanical, not servo   | sim/flight_controls/pitch_trim_up_mech   |
| Pitch trim down - Mechanical, not servo | sim/flight_controls/pitch_trim_down_mech |
| Roll trim left                          | sim/flight_controls/aileron_trim_left    |
| Roll trim right                         | sim/flight_controls/aileron_trim_right   |
| Yaw trim left                           | sim/flight_controls/rudder_trim_left     |
| Yaw trim right                          | sim/flight_controls/rudder_trim_right    |

____

