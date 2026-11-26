# OpenStreetMap-derived data — Katrina's Mystic Visitors Guide

Map, place and walking-path data in this app come in part from OpenStreetMap.
That OpenStreetMap-derived part is made available here under the
**Open Database License 1.0** (`LICENSE-ODbL-1.0.txt`,
opendatacommons.org/licenses/odbl/1-0/).

**Attribution:** © OpenStreetMap contributors.
**Questions or requests:** contact@destructiveaigurus.com

## What this export covers
- App version **20261017.1**. Exported 2026-11-25.
- The same data ships in the iPhone edition built from this release's content.

## Files
| File | What it holds |
|---|---|
| `walking-route-network.sqlite` | The walking-route network the app uses (46,349 edges, 43,087 nodes). |
| `walking-route-network.geojson` | The same network as GeoJSON LineStrings (WGS 84; `source`/`target` are node ids, `length_m` in metres, `mtfcc` = the segment's feature class). |
| `places-osm-derived.geojson` / `.csv` | 457 places of OpenStreetMap origin, numbered 1–457, with only their OpenStreetMap-derived fields (212 with coordinates). |
| `export-manifest.json` | Counts and the SHA-256 of every file. |
| `SHA256SUMS` | Checksums of every file in this folder. |

## Which data is included
- **The walking-route network, as a whole.** Some of its paths come from
  OpenStreetMap and some from public-domain sources; they cannot all be told
  apart, so the whole network is offered under ODbL.
- **Places of OpenStreetMap origin:** 32 lodging places
  imported from OpenStreetMap, and 425
  places first created from OpenStreetMap data. Only fields that still derive
  from OpenStreetMap are included; values from other sources are left out.
  `osm_origin` says which: `osm_lodging` (the fields that still match
  OpenStreetMap) · `osm_name_category_location` (name, category, coordinates)
  · `osm_name_category` (name and category).
- **Not included:** the rest of the app's database (stories, narration,
  images, audio and other content), which is a separate, independent
  collection under ODbL §4.5; and the map tiles, which are a Produced Work
  (ODbL §4.3) and carry the attribution above.
