# FDFPV Itaipu data

Terrain tiles, imagery and map data for the Itaipu map of
[FDFPV](https://fdflabs.github.io/fdfpv/): the Itaipu Dam on the Parana
River at real scale, a 10.24 km hero square around the dam and a 40.96 km
ring of terrain around it. The simulator fetches these files at run time;
this repository is served as a static site for that.
FDFPV and this data repository are made by [fdflabs.com](https://fdflabs.com).

The format is the contract in the simulator's `docs/ITAIPU-PLAN.md`
(section 14), and `manifest.json` lists every file with its checksum. The
files are built by `tools/itaipu/` in the simulator's repository
(github.com/fdflabs/fdfpv); do not edit them by hand.

## Attribution

Wherever the map is shown:

- Elevation: ANADEM v1, Laipelt et al. 2024, Remote Sensing 16(13):2321, ANA / IPH-UFRGS, CC BY 4.0, resampled and edited
- Copernicus DEM GLO-30: (c) DLR e.V. 2010-2014 and (c) Airbus Defence and Space GmbH 2014-2018 provided under COPERNICUS by the European Union and ESA; all rights reserved
- Contains modified Copernicus Sentinel data 2025 and 2026, processed by ESA
- (c) OpenStreetMap contributors, ODbL, openstreetmap.org/copyright

## Sources and licences

Each file is under the licence of the source it was made from; `LICENCE.md`
has the terms.

- Elevation: ANADEM v1 (Agencia Nacional de Aguas e Saneamento Basico and
  IPH-UFRGS; Laipelt et al. 2024, "ANADEM: A Digital Terrain Model for
  South America", Remote Sensing 16(13):2321, doi:10.3390/rs16132321),
  CC BY 4.0. Changed: resampled to 30 and 10 m, water beds carved under
  the reservoir and the river, the dam's embankments raised and its
  concrete footprints flattened.
- Water levels and extents, canopy height: Copernicus DEM GLO-30, (c) DLR
  e.V. 2010-2014 and (c) Airbus Defence and Space GmbH 2014-2018 provided
  under COPERNICUS by the European Union and ESA; all rights reserved.
  Used under the Copernicus DEM licence.
- Colour and ground masks: contains modified Copernicus Sentinel data
  2025 and 2026, processed by ESA (Sentinel-2 L2A, via Element 84 Earth
  Search).
- Buildings, roads, power lines, trees, land use, and the dam's axes and
  footprints: (c) OpenStreetMap contributors. `osm/*.json` is a derived
  database of OpenStreetMap and is made available under the Open
  Database License 1.0 (openstreetmap.org/copyright); each feature keeps
  its OpenStreetMap id.
- The dam's dimensions: Itaipu Binacional's published figures
  (www.itaipu.gov.br/energia), cited by page in `dam.json`. Facts, not
  text; no Itaipu Binacional logo or branding is used.

Each source's download URL, dates, retrieval time and checksum are in
`manifest.json`.
