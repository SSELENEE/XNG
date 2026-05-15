# XNG Research Desk v0.9.5 — Streamlit Cloud Safe

Fixes Streamlit Cloud deployment failure caused by Fiona/GDAL.

Changes:
- Removed geopandas/fiona/pyproj dependency from NOAA shapefile engine.
- NOAA 6-10D / 8-14D use pyshp + shapely only.
- Still reads NOAA CPC shapefile attributes directly: `Cat`, `Prob`, geometry.
- No screenshot OCR/crop/warp.

Run:
```bash
streamlit run app.py
```
