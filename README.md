# chm_intercomparison
Global CAnopy height Model Intercomparison (CAMI) and Validation Exercise

### Keywords
CAMI; Validation; LiDAR; GEDI; Canopy Height Model; Forest; 3D; lastools; WRI; Meta

### Abstract
Machine learning methods have facilitated the extrapolation of estimates of canopy height from optical imagery in locations where direct observations (LiDAR, RADAR) are unavailable, significantly improving our ability to understand forest structure and estimate aboveground biomass at global scales. Quantifying the uncertainty of these predictions, and thus determining credibility of models, is critical for users to select the most useful model for their application. To date, no independent intercomparison and validation of available, wall-to-wall Canopy Height Models (CHMs) has been published. Presented here is a novel, comprehensive, robust, fair, and transparent methodology for conducting a model intercomparison and validation of the existing, publicly available catalogue of CHMs, at the time of writing. The intended purpose of the CAnopy height Model Intercomparison (CAMI) exercise is for it to be repeatedly conducted in phases, and scope expanded, as model developers release new, or improve existing models. The study compares 4 CHMs with globally exhaustive coverage, generated for 2019-2020 (inclusive) leaf-on season using various machine learning methods, across 6 globally-representative, well-established scientific forest plots (FBRM sites) with ALS and GEDI footprint coverage. CHMpot is found to be the most credible model of the ensemble, with high mean prediction accuracy (RMSE=9.30m, MAE=7.36m), low mean bias (ME=0.49m), and strong agreement with CHMpau. When validated against ALS, all models performed to within 40-60% of the observed height for heights within the optimal range, which was found to be 25-40m for best ensemble prediction accuracy.

### Key Figures
![fig1](https://github.com/user-attachments/assets/d7304584-7e34-48ec-b953-0077f5d684e8)
*Figure 1: ALS point cloud (.laz) processing stages for a tile (290m by 290m) in Paracou, French Guiana (PARA) to generate canopy height model. (a) 3D point cloud visualised as raw z coordinate values. (b) Ground point classification (.laz) using lasground defaul settings. (c) Canopy height model generation (.tif) at 1m resolution and RH98 (Li et al., 2023) using lascanopy64, which subtracts ground height from canopy top height at the 98th return percentile.*

![fig2](https://github.com/user-attachments/assets/3e766857-3dcf-4398-bab4-e460052d6074)
*Figure 2: Visual intercomparison of model predictions at original ground sampling resolutions, and GEDI RH98 return, against ALSderived CHMs. Visualised for a small sample of the plot extent at all sites, for equally scaled tiles (excluding WYTH, due to smaller total plot area)*

![fig3](https://github.com/user-attachments/assets/14598926-f0a7-451c-be33-bb99482be6eb)
*Figure 3: ALS-derived canopy height (m) versus predicted canopy height (m), by model. Visualised per pixel, where pixel extent is clipped to GEDI L2A RH98 footprint for all sites, and pixels are grouped in 1m by 1m height bins to derive pixel frequency. Line at y=x represents an accurate prediction of quasi-ground truth height (ALS), and n represents total pixel count by site.*

