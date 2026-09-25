# Outdoor Wood Multi-Gym — Slot-10

Canonical GitHub repository for the **8 ft × 8 ft outdoor wooden multi-gym project**.

## Project goal

Design a low-cost, weather-tolerant multi-gym that fits inside an 8×8 ft square. One rear side sits against a wall and is not accessible from behind. The design combines purchased low-cost equipment with DIY pressure-treated lumber/steel modules.

The rear bench/squat structure is planned around **6×6 pressure-treated rack uprights**, steel pipe bar rests/safeties, and a common removable accessory receiver. The gym standardizes plate-loaded equipment on **2-in Olympic plates**.

## Mandatory working procedure

Before changing this project:

1. Read `PROJECT_MEMORY.md`.
2. Read `OUTDOOR_GYM_ROADMAP.md`.
3. Read `docs/DECISION_MATRIX.csv` and `docs/COMMON_CONSTRUCTION_STANDARDS.md`.
4. Preserve the 8×8 footprint and inaccessible rear-wall constraint unless the user explicitly changes them.
5. Do not silently weaken safety-critical hardware, post sizes, anchors, pivots, safeties, or cable mounts.
6. Update `PROJECT_MEMORY.md` and the roadmap after any major design decision.
7. Generated CAD is a fabrication starting point, not stamped engineering. Safety-critical components require verification for the actual site and intended loads.

## Repository layout

- `src/generate_outdoor_gym_v2.py.gz` — compressed parametric CadQuery generator.
- `docs/` — decisions, construction standards, purchased-item interfaces, and build manual.
- `.github/workflows/build-cad.yml` — GitHub Actions CAD build.
- Generated STEP/STL/GLB/drawings are produced as a workflow artifact rather than committed as large generated binaries.

## CAD build

The generator uses **CadQuery**, **trimesh**, and **CairoSVG**. Pushes that change CAD source or build docs trigger the CAD workflow. The workflow regenerates the full v2 package and uploads it as a downloadable GitHub Actions artifact.

## Current stage

Detailed v2 prototype package exists. The next design phase is to validate each module one at a time, starting with the site/floor and master frame, then rack safeties, purchased-bench fit, pulley anchors, leg press, and removable accessories.

See `OPEN_SOURCE_REFERENCES.md` for open-source tools/projects we can reuse or study.
