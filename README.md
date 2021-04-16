# odu_test
ODU Map for Mosaic-Sumo-CARLA

Using `config.py` to load OpenStreetMap file directly into CARLA.
```
python3 config.py --osm-path=odu_test.osm
```
Or load OpenDRIVE file into CARLA:
```
python3 config.py -x odu_test.xodr
```

Move `odu_test` folder to `scenarios` folder in MOSAIC.

Execute `odu_test` scenario:
```
mosaic.bat -s odu_test -v
```
