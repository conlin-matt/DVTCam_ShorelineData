# Argus-derived shorelines from the DVT Camera at Kennedy Space Center, FL #

This repo contains Argus-derived shorelines from the DVT Cam deployed at NASA-Kennedy Space Center from mid 2011 to mid 2012. Details of data processing and results can be found in:

Conlin, M. P., Adams, P. N., Plant, N. G., Jaeger, J. M., & MacKenzie, R. (2019). Daily to Decadal Variability of Beach Morphology at NASA-Kennedy Space Center: Storm Influences Across Timescales. *Proceedings of the Coastal Sediments 2019*. World Scientific Publishing.


### Files in the repo ###
1) **shorelineManualResults_daily_withY.mat**

  * This mat file loads a Matlab structure (called slPosStruct) that contains the manually extracted shoreline observations. The structure contains four fields, where each row is an observation:
    * Date: The (Matlab datetime) date when the shoreline was found
    * sl: The cross-shore position of the shoreline at 161 longshore locations 
    * tide: The observed tidal elevation at the time of the shoreline observation
    * y: The 161 longshore positions at which shorelines are extracted

  * The longshore variable shoreline position at one time can be plotted 	by, for example, executing: `plot(slPosStruct(i).sl,slPosStruct(i).y)`

2) **shorelineManualResults_lcp.mat**

  * This mat file loads the camera's Lens Calibration Profile (lcp) Matlab structure (standard CIRN processing format).
  
3) **shorelineManualResults_beta.mat**

  * This mat file loads the beta vector (geometry solution) used to rectify the camera's images (standard CIRN processing format).

