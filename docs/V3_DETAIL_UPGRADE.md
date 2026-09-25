# v3 detail upgrade

The v2 models were useful as layout/space-claim models but were not visually detailed enough for fabrication review. The user correctly rejected them as "just blocks."

## v3 modeling standard

The v3 master assembly is rebuilt as separate named components rather than one compound. It includes approximately 311 parts and visibly models:

- floor rims, joists, blocking, deck sheets and rubber mat seams;
- 4×4/6×6 lumber at actual dressed dimensions;
- drilled rack and safety-upright hole rows;
- steel reinforcement straps with matching holes;
- bolt shafts, hex heads, nuts and washers at major connections;
- hollow pipe bar rests and safeties with retainers and saddle pads;
- Olympic bar, sleeves and collars;
- a more detailed purchased-bench proxy with steel frame, pads, hinge, ladder, feet and wheels;
- pull-up-bar plates/bolts;
- pulley wheels, axles, cables, loading pin, plates and lat bar;
- hollow universal receiver, base plate, anchor bolts and removable pin;
- dip/knee-raise hardware and pads;
- plate-storage horns, Olympic plates and spare-bar holder;
- landmine base/yoke/pivot/sleeve;
- a significantly more detailed leg press with base rails, laminated arms, pivot hardware, side plates, loading horns, plates, footplate, stops and safety pin;
- band anchor proxies and slant board.

## File outputs

- `MASTER_8x8_GYM_DETAILED_V3.step` — componentized STEP assembly.
- `MASTER_8x8_GYM_DETAILED_V3.glb` — colored phone-viewable model.
- `RACK_SAFETY_DETAIL_V3.glb` — rack/bench/safety closeup.
- `LEG_PRESS_DETAIL_V3.glb` — leg press closeup.
- `PULLEY_RECEIVER_DETAIL_V3.glb` — cable/receiver closeup.

## Remaining limitation

Purchased equipment is still a detailed **proxy** until the exact Amazon model is chosen and measured. Do not treat proxy mounting dimensions as manufacturer dimensions.

The next refinement should make each BUILD module its own detailed component assembly and then replace purchased proxies one-by-one as exact products are selected.
