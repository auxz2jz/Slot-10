# PROJECT_MEMORY — Outdoor Wood Multi-Gym

**Repository:** auxz2jz/Slot-10  
**Project:** Outdoor 8×8 Wooden Multi-Gym  
**Status:** Detailed v2 prototype / pre-fabrication refinement

## Permanent constraints

- Maximum planned footprint: **8 ft × 8 ft (96 × 96 in)**.
- One entire rear side is against a wall. Nothing may require routine access behind that side.
- Equipment must operate primarily inside the square or, at minimum, from the other three open sides.
- Low cost is a primary goal: buy inexpensive commercial equipment when it is cheaper/more practical; build the rest from pressure-treated lumber, steel pipe/shaft, plywood, and purchased hardware.
- Outdoor exposure is expected. Use pressure-treated/exterior materials and corrosion-compatible hardware.
- Plate-loaded equipment standard: **2-in Olympic plates**.
- Rear bench/squat rack uprights: use **6×6 pressure-treated posts** as the current baseline, not 4×4.
- Bar rests and bench/squat safeties: DIY steel pipe/pin system through reinforced wooden uprights rather than expensive commercial J-hooks.
- Floor/site may begin over dirt; planned solution is drainage/compacted aggregate + raised PT platform + rubber/stall-mat impact surface.
- Purchased padded/cable items should be removable/stored under cover when practical.

## Core layout

- Rear/wall side: bench press + squat rack facing inward.
- Bench runs perpendicular from rear rack toward center/front.
- Front/center: removable leg-press and bench-receiver attachments.
- Open sides: dip, band/cable mounts, landmine, storage, bodyweight attachments.
- Overhead: purchased pull-up bar and pulley anchors.
- Common removable receiver target envelope: 2.5-in square steel receiver accepting a 2-in attachment shank, retained by a rated 5/8-in pin.

## Current BUY / BUILD decisions

The authoritative complete list is `docs/DECISION_MATRIX.csv`.

Key BUY items: adjustable FID bench, pull-up bar, high/low pulley kit, landmine pivot, adjustable step, Olympic bar/plates, Olympic dumbbell handles, cable-handle bundle, assistance bands, belt-squat/dip belt, hip-thrust pad, landmine row handle, collars, resin deck box, and rated safety/attachment hardware.

Key BUILD items: integrated bench/squat rack, leg press, combined leg extension/curl, preacher curl, dip station, band anchors, integrated weight/bar storage, outdoor platform, seated-row foot brace, knee-raise station, push-up handles, back extension, crossover mounts, Nordic anchor, seated calf raise, lat thigh hold-down, slant board, bar rests/safeties.

Existing equipment is reused for shoulder press, standing calf raise, pec/rear-delt cable flys, deadlift/barbell rows, belt squat, and hip thrust.

## Safety rules that must not be lost

- Do not use deck skin alone as a structural attachment for rack, pivot, or receiver loads.
- Use through-bolts with locking nuts and large washers/backing plates at safety-critical joints.
- Hardware touching pressure-treated lumber must be compatible with the preservative (appropriate hot-dip galvanized or stainless).
- Use steel at bar rests, safeties, pivots, loading horns, and bodyweight handles.
- Use bushings/bearings at moving pivots rather than letting steel shafts grind directly in wood.
- Purchased bench/pulley dimensions are placeholders until the exact models are bought and physically measured.
- Verify safety-pipe height so a failed bench press is caught above the user's chest/neck while still allowing normal range of motion.
- Rack/safeties, leg-press pivot/stops, cable anchors, bodyweight mounts, footings/anchors, welds, and fastener grades are safety-critical and need load/site verification before heavy use.
- Progressive proof testing: unloaded first, then increasing loads while standing clear.

## CAD source

The v2 generator is a CadQuery Python program. In GitHub it is stored as five base64 chunks (`src/generator.b64.part00` through `part04`) containing a gzip-compressed copy of the verified generator. The Actions workflow concatenates, decodes, expands, syntax-checks, and executes it. Local/chat generation has already been verified successfully.

## Change-control / anti-loop procedure

1. Read this file before work.
2. Change one subsystem at a time.
3. Record exact dimensions/hardware changes in the corresponding roadmap item.
4. Rebuild CAD after source changes.
5. Compare generated package contents before accepting the change.
6. Never repeatedly redesign a subsystem without stating what failed and what changed.
7. Keep BUY-item interfaces generic until the exact purchased product is selected; then add its measured envelope/hole pattern without assuming Amazon listing dimensions are exact.
