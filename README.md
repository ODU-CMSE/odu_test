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

Test:
```
python3 spawn_npc_sumo.py -n 100 --sumo-gui --tls-manager sumo
```

```
python3 run_synchronization.py odu_test.sumocfg --sumo-gui --tls-manager sumo
```
