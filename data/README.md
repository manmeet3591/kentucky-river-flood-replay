# Data

Open data behind the Kentucky River flood replay. Everything here comes from public sources and may be reused with the attributions below.

## Gauge records (`usgs/`)

Hourly gage height in feet from USGS instantaneous (15-minute) data, in local time (EDT for April, EST for February).

| File | USGS station | Status |
|---|---|---|
| 03287500_..._2025-04_hourly.csv | Kentucky River at Lock 4, Frankfort | Approved |
| 03282000_..._2025-02_hourly.csv | Kentucky River at Lock 14, Heidelberg | Approved |
| 03282120_..._2025-02_hourly.csv | Kentucky River at Lock 12 near Irvine | Approved |
| 03280000_..._2025-02_hourly_provisional.csv | North Fork Kentucky River at Jackson | Provisional, subject to revision |

Source: U.S. Geological Survey, Water Data for the Nation (https://waterdata.usgs.gov). USGS data are in the public domain.

## Satellite water maps (`opera_layers/`)

Transparent PNG renderings of the NASA/JPL OPERA Dynamic Surface Water Extent from Sentinel-1 (DSWx-S1) v1.0 water classification layer (B01_WTR), with county boundaries. Colors: blue open water, green inundated vegetation, orange flood water seen only on April 6, light blue water on both dates, gray water on April 13 only, translucent gray not imaged.

Source granules:

- `OPERA_L3_DSWx-S1_T16SFH_20250406T234025Z_20250407T102148Z_S1A_30_v1.0_B01_WTR.tif`
- `OPERA_L3_DSWx-S1_T16SFH_20250413T233211Z_20250414T133032Z_S1A_30_v1.0_B01_WTR.tif`
- `OPERA_L3_DSWx-S1_T16SGG_20250217T234000Z_20250221T055027Z_S1A_30_v1.0_B01_WTR.tif`
- `OPERA_L3_DSWx-S1_T16SGH_20250406T234025Z_20250407T102148Z_S1A_30_v1.0_B01_WTR.tif`
- `OPERA_L3_DSWx-S1_T17SKB_20250217T234000Z_20250221T055027Z_S1A_30_v1.0_B01_WTR.tif`

Citation: OPERA Dynamic Surface Water Extent from Sentinel-1 (Version 1), NASA PO.DAAC, doi:10.5067/OPDSWS1-L3V1. Contains modified Copernicus Sentinel data (2025).

## Overlays and statistics

- `map_overlays.json`: marker positions as fractions of image width and height, the western edge of the April 13 look, zoom boxes and map extents in km.
- `stats_april_2025.json`, `stats_february_2025.json`: acquisition times, tile coverage, gauge stages at each pass and water areas used on the page.

National Weather Service flood categories come from the NWS Advanced Hydrologic Prediction Service. County boundaries are from the U.S. Census Bureau.
