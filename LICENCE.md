# Licences

The files in this repository are data, each under the licence of the
source it was made from. None of them is under the simulator's GPL; the
simulator (github.com/fdflabs/fdfpv) is GPLv3 and uses them as data.

| Files | Source | Licence |
| --- | --- | --- |
| `0/`, `1/`, `2/`, `3/`, `hero/` (elevation) | ANADEM v1, ANA / IPH-UFRGS | CC BY 4.0, https://creativecommons.org/licenses/by/4.0/ ; changed as README.md says |
| the same tiles' water beds, `water.json`, `canopy/` | Copernicus DEM GLO-30 | Copernicus DEM licence (free use, copying, modification and redistribution, with the notice below) |
| `imagery/`, `masks/` | Sentinel-2 L2A (and OpenStreetMap in `masks/`) | Copernicus Sentinel data terms, Regulation (EU) 1159/2013: free, full and open; ODbL for the OpenStreetMap part |
| `osm/` | OpenStreetMap | Open Database License 1.0, https://opendatacommons.org/licenses/odbl/1-0/ |
| `dam.json` | OpenStreetMap (axes, footprints) and Itaipu Binacional's published figures | ODbL 1.0 for the geometry; the figures are cited facts |
| `manifest.json`, `README.md`, `LICENCE.md` | this project | CC0 |

## Notices

- Elevation: ANADEM v1, Laipelt et al. 2024, Remote Sensing 16(13):2321, ANA / IPH-UFRGS, CC BY 4.0, resampled and edited
- Copernicus DEM GLO-30: (c) DLR e.V. 2010-2014 and (c) Airbus Defence and Space GmbH 2014-2018 provided under COPERNICUS by the European Union and ESA; all rights reserved
- Contains modified Copernicus Sentinel data 2025 and 2026, processed by ESA
- (c) OpenStreetMap contributors, ODbL, openstreetmap.org/copyright

`osm/*.json` and the OpenStreetMap-derived geometry in `dam.json` and
`masks/` are a derived database of OpenStreetMap, offered here under the
ODbL 1.0: you may copy, distribute and adapt them as long as you
attribute OpenStreetMap and its contributors and keep any adapted
database under the ODbL. A map drawn from them (a produced work) may be
under any licence, with the attribution above shown where it is used.
