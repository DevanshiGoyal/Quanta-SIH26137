# Traffic Dataset Storage

This directory contains the real-world traffic datasets and generated artifacts used by Quanta-SIH26137.

## Dataset policy

The actual datasets are **not committed to normal Git history** because the complete local data directory is approximately 1.5 GB.

The repository stores the code and metadata required to reproduce the datasets, while the large raw and generated artifacts remain outside normal Git tracking.

## Datasets

### METR-LA

METR-LA contains traffic-speed observations from 207 traffic sensors in the Los Angeles metropolitan area at approximately 5-minute resolution.

Local expected structure:

```text
data/raw/METR-LA/
├── metr-la.h5
└── graph/
    ├── graph_sensor_ids.txt
    ├── graph_sensor_locations.csv
    └── distances_la_2012.csv