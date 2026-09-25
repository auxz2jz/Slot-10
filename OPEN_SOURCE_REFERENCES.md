# Open-source GitHub resources

We can use these projects as tooling/reference dependencies. Do not copy code or CAD from unrelated projects without checking its license and relevance.

## CadQuery
- Repository: https://github.com/CadQuery/cadquery
- Purpose: Python parametric CAD scripting framework based on OpenCascade/OCCT.
- Project use: **Primary generator technology for this gym.** STEP/STL and drawing geometry are generated from Python.

## FreeCAD
- Repository: https://github.com/FreeCAD/FreeCAD
- License reported by GitHub: LGPL-2.1
- Purpose: free/open-source multi-platform parametric CAD.
- Project use: recommended desktop viewer/editor for STEP files and manual inspection/dimension checking.

## OpenSCAD
- Repository: https://github.com/openscad/openscad
- Purpose: script-driven solid CAD.
- Project use: possible future lightweight secondary generator for simple brackets/templates; not currently the source of truth.

## trimesh
- Repository: https://github.com/mikedh/trimesh
- License reported by GitHub: MIT
- Purpose: Python mesh processing.
- Project use: current CadQuery build pipeline uses it to convert/export mesh/GLB viewing files.

## Reuse policy
- Prefer using these projects as installed dependencies/tools.
- If we later reuse code snippets or models from a third-party repository, record the exact repository, path, commit, and license here before incorporating it.
- Avoid importing random home-gym CAD merely because it looks similar; safety-critical geometry must be understood and verified.
