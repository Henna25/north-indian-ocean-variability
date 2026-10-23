# Seasonal and Interannual Variability of Physical Parameters in the Northern Indian Ocean

Research internship at the **CSIR-National Institute of Oceanography (NIO), Goa**, Physical Oceanography Division
Supervisor: **Dr. Akhil Valiya Parambil** · May – July 2024
Author: **Fathimathul Hennath P H** (M.Sc. Oceanography, Cochin University of Science and Technology)

---

## Overview

The northern Indian Ocean is landlocked to the north and forced by seasonally reversing monsoon winds, which makes its upper-ocean variability unlike that of any other basin. This project examines:

1. **Seasonal variability**: monthly climatologies (1993–2021) of sea surface temperature (SST), sea surface salinity (SSS), mixed layer depth (MLD), surface currents, winds and precipitation, contrasting the **Arabian Sea (AS)** and the **Bay of Bengal (BoB)**.
2. **Interannual variability**: the **Indian Ocean Dipole (IOD)**, using the Dipole Mode Index (DMI), with a closer look at the strong positive IOD events of **1997** and **2019**.

**Study region:** 40°E–100°E, 0°–25°N

![Monthly climatology of SST and winds](figures/sst_wind_climatology.png)

---

## Data

| Variable | Source | Period |
|---|---|---|
| SST, SSS, MLD | [ORAS5 Ocean Reanalysis](https://cds.climate.copernicus.eu/) (ECMWF / Copernicus) | 1993–2021, monthly |
| Surface winds | [ERA5 Reanalysis](https://cds.climate.copernicus.eu/) (ECMWF) | 1993–2021, monthly |
| Surface currents | [OSCAR](https://podaac.jpl.nasa.gov/) (Earth & Space Research / NASA PO.DAAC) | monthly |
| Precipitation | [GPCP](https://psl.noaa.gov/data/gridded/data.gpcp.html) (NOAA PSL) | 1996–2021 |

The data files are not included in this repository because of their size. They can be downloaded from the links above.

---

## Methods

- **Monthly climatology and anomalies.** Anomaly = monthly value − climatological monthly mean.
- **Box averages** over the Arabian Sea and the Bay of Bengal, used to compare the seasonal cycles of the two basins.
- **Dipole Mode Index (DMI)** (Saji et al., 1999): the SST anomaly of the western box (50°–70°E, 10°S–10°N) minus that of the eastern box (90°–110°E, 10°S–0°).
- **Z-score normalisation**, (x − μ) / σ, used to compare indices on a common scale.

---

## Notebooks

| Notebook | Description |
|---|---|
| `currents_climatology.ipynb` | Monthly climatology of SSS with surface currents |
| `mld_and_wind.ipynb` | Monthly climatology of mixed layer depth with surface winds |
| `arabian_sea_physical_properties.ipynb` | Box-averaged seasonal cycles of SST, SSS, MLD, currents, precipitation and wind in the AS and BoB |
| `time_series_plots.ipynb` | Time series of physical parameters for the AS and BoB |
| `d20_climatology.ipynb` | Climatology of the 20 °C isotherm depth (D20), a proxy for thermocline depth |
| `sla_climatology.ipynb` | Climatology of sea level anomaly |
| `iod_dipole_mode_plots.ipynb` | DMI time series (1993–2021), and SST anomaly maps for the 1997 and 2019 positive IOD events |
| `iod_climate_indices.ipynb` | Climate indices and west/east SST anomalies for the positive IOD years |
| `olr_east_anomaly.ipynb` | Outgoing longwave radiation (OLR) anomaly over the eastern box (convection proxy) |
| `olr_west.ipynb` | OLR anomaly over the western box |

**Requirements:** Python 3 with `xarray`, `numpy`, `pandas`, `matplotlib` and `cartopy`.

---

## Key Findings

**Seasonal cycle**
- **SST** peaks in the spring inter-monsoon (Mar–May, ~30 °C) and falls during the summer monsoon. Cooling is stronger in the Arabian Sea (30 → 27 °C) than in the Bay of Bengal (30 → 28.5 °C), because of wind mixing, upwelling and reduced solar heating.
- **SSS** is consistently higher in the Arabian Sea (~36 psu), driven by evaporation and Red Sea / Persian Gulf outflow. The Bay of Bengal is much fresher (~33 psu) because of heavy rainfall and Ganga–Brahmaputra runoff.
- **MLD** deepens to more than 60 m in the Arabian Sea during the summer monsoon (wind mixing) and to more than 55 m in winter (convective mixing). It stays shallow (30–40 m) in the stratified Bay of Bengal.
- **Precipitation** is higher over the Bay of Bengal throughout the year, peaking at about 8 mm/day during the summer monsoon.

![Seasonal cycles in the Arabian Sea and Bay of Bengal](figures/as_bob_time_series.png)

**Indian Ocean Dipole**
- Positive IOD years: 1994, 1997, 2006, 2015 and 2019. Negative IOD years: 1996, 1998, 2010 and 2016.
- In **1997**, cooling in the eastern box dominated. In **2019**, warming in the western box dominated.
- The onset, peak month, duration and east–west balance of the anomalies vary markedly from event to event. This points to different driving mechanisms behind individual IOD events.

![Dipole Mode Index 1993–2021](figures/dmi_1993_2021.png)

---

## Key References

- Saji, N. H., Goswami, B. N., Vinayachandran, P. N., & Yamagata, T. (1999). A dipole mode in the tropical Indian Ocean. *Nature*, 401, 360–363.
- Shankar, D., Vinayachandran, P. N., & Unnikrishnan, A. S. (2002). The monsoon currents in the north Indian Ocean. *Progress in Oceanography*, 52, 63–120.
- Schott, F. A., Xie, S.-P., & McCreary, J. P. (2009). Indian Ocean circulation and climate variability. *Reviews of Geophysics*, 47, RG1002.
- Shenoi, S. S. C., Shankar, D., & Shetye, S. R. (2002). Differences in heat budgets of the near-surface Arabian Sea and Bay of Bengal. *JGR*, 107(C6).

---

## Contact

**Fathimathul Hennath P H** · [hennathfathimathul@gmail.com](mailto:hennathfathimathul@gmail.com) · [LinkedIn](https://linkedin.com/in/fathimathul-hennath-ph-b91066206) · [Website](https://henna25.github.io/Henna25/)
