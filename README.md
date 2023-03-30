# SMAP soil moisture download and process

GEE code: https://code.earthengine.google.com/6ab400ae15808b9298f870fc61f18743

This dataset is being superseded by SPL4SMGP.007

The NASA-USDA Enhanced SMAP Global soil moisture data provides soil moisture information across the globe at 10-km spatial resolution. This dataset includes: surface and subsurface soil moisture (mm), soil moisture profile (%), surface and subsurface soil moisture anomalies (-).

The dataset is generated by integrating satellite-derived Soil Moisture Active Passive (SMAP) Level 3 soil moisture observations into the modified two-layer Palmer model using a 1-D Ensemble Kalman Filter (EnKF) data assimilation approach. Soil moisture anomalies were computed from the climatology of the day of interest. The climatology was estimated based on the full data record of the SMAP satellite observation and the 31-day-centered moving-window approach. The assimilation of the SMAP soil moisture observations help improve the model-based soil moisture predictions particularly over poorly instrumented areas of the world that lack good quality precipitation data.

This dataset was developed by the Hydrological Science Laboratory at NASA's Goddard Space Flight Center in cooperation with USDA Foreign Agricultural Services and USDA Hydrology and Remote Sensing Lab.

See: https://developers.google.com/earth-engine/datasets/catalog/NASA_USDA_HSL_SMAP10KM_soil_moisture#description

## Processing

Processing was done in R to convert daily data into monthly and annual data. Subsequently, graphic products such as annual maps and animation were generated. An interesting finding in these data analyzed for the Tacurembó river basin is that in the driest years (2021 and 2022) the zones where the eucalyptus plantations are located had lower values of soil moisture in the subsurface, indicating greater consumption by transpiration. More evidence will be collected to assess this scenario.

Let's go ahead

#### Maps

![Rplot01](https://user-images.githubusercontent.com/60663771/228826172-647f45ee-f9fd-4593-a9fa-86d58a658ba6.jpeg)

#### Animation

https://user-images.githubusercontent.com/60663771/228825762-d0b166e0-a2b4-439d-8b85-120c145a3f2e.mp4

