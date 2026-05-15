# XNG Research Desk v0.9.4 — NOAA Shapefile Primary

Patch scope:
- NOAA 6-10D and NOAA 8-14D now use the same NOAA CPC shapefile primary engine.
- Screenshot/color/warp NOAA engine is no longer used for scoring.
- Screenshot upload remains only as optional archive/visual reference.
- CME / News / Weekly Storage / Monthly STEO logic is unchanged.

## Run

```bash
cd ~/Downloads/xng_research_desk_v0_9_4_noaa_shapefile && python3 -m venv .venv && source .venv/bin/activate && pip install -r requirements.txt && streamlit run app.py
```

## NOAA usage

For both NOAA 6-10D and NOAA 8-14D:
1. Upload all NOAA shapefile sidecar files: `.shp`, `.dbf`, `.shx`, `.prj`, `.cpg`, etc.
2. Click `Auto Fill from NOAA Shapefile`.
3. Review preview JSON.
4. Click `Apply NOAA Shapefile to Fields`.
5. Save/confirm normally.

## Required NOAA shapefile fields
- `Cat`
- `Prob`
- `geometry`

Optional metadata:
- `Fcst_Date`
- `Start_Date`
- `End_Date`
