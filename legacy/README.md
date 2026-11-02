# legacy/

Earlier versions of the three notebooks (December 2024), kept as they were. They are not maintained.

| File | What it was |
|---|---|
| `01_Intro_To_Python_Gis.ipynb` | Python basics with an "expedition" theme. It ran, but `calculate_distance` was Pythagoras on degrees (Buenos Aires–Córdoba = 6.6, no unit) and never printed the result. |
| `02_Working_With_Data.ipynb` | pandas walkthrough. Never executed: it failed at the second code cell reading `expedition_data.csv`, `camp_locations.xlsx` and `sensor_data.json`, which never existed. Later cells used undefined names (`data`) and APIs that don't exist (`.dt.season`) or are deprecated (`resample('M')`, chained `fillna(inplace=True)`). |
| `03_Intro_To_Geodata.ipynb` | GeoPandas walkthrough. Most cells only defined functions that were never called; the folium cell used an undefined `gdf`. Its "5 km" buffers were drawn in EPSG:3857, which at Buenos Aires' latitude measure about 4.1 km. |

A 5 MB GIF (Landsat timelapse of tree cover loss in Sinop, Brazil) was in `notebooks/` without being used anywhere; it was removed from the tree and is still in the history at commit [`fa33cbb`](https://github.com/oechenique/python-gis-basics/tree/fa33cbb/notebooks).

The current notebooks in [`notebooks/`](../notebooks/) keep the same paths, so old Colab links still work, and they run end to end.
