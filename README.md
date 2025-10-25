# Integrating Map Accuracy and Sampling Efficiency for Cropland Area Estimation

This repository contains the code and data for the research paper "Integrating Map Accuracy and Sampling Efficiency for Cropland Area Estimation".

## Description

This project implements and combines several methods to improve the precision of cropland area estimates. The core of the work is presented in the `Notebook.ipynb` Jupyter Notebook.

The methods implemented are:
- Unbiased stratified estimators for accuracy estimation from [Stehman (2014)](https://www.tandfonline.com/doi/full/10.1080/01431161.2014.930207).
- Relative efficiency of maps from [Skakun (2025)](https://www.sciencedirect.com/science/article/pii/S0034425725002093).
- A stratified estimator for area estimation from [Olofsson et al. (2014)](https://www.sciencedirect.com/science/article/pii/S0034425714000704).

## Notebook

The main analysis is in `Notebook.ipynb`. This notebook covers:
1.  **Land cover maps accuracy assessment**: Calculates overall, user's, and producer's accuracy for different land cover maps.
2.  **Relative efficiency and Area estimation**: Determines the most efficient map for sampling and estimates cropland area.
3.  **Visualization**: Creates plots for error matrices, relative efficiency, and comparison of area estimates.



## Data

The `data/` directory contains the datasets used in the analysis:

- `reference_sample_pixel_values.csv`: Reference sample pixel values for different land cover maps [input].
- `binary_mapped_area.csv`: Mapped area (pixel-count) per stratum for different maps [input].
- `area_estimation_refrence_samples.csv`: Reference samples for area estimation [input].
- `land_use_data.csv`: External land use statistics (e.g., from FAOSTAT) [input].
- `accuracy_assessment_results.csv`: The results of the accuracy assessment [output].


## Citation

If you use this work, please cite it as follows:

```
@article{authorintegrating,
  title={Integrating Map Accuracy and Sampling Efficiency for Cropland Area Estimation},
  author={},
  journal={},
  volume={XXX},
  pages={YYY-ZZZ},
  year={},
  publisher={}
}
```

## Credits

- [NASA Harvest crop-mask - compare_cover module](https://github.com/nasaharvest/crop-mask/blob/master/src/compare_covermaps.py)

## References

- Skakun, S. (2025). The impact of map accuracy on area estimation with remotely sensed data within the stratified random sampling design. *Remote Sensing of Environment*, 326, 114805.
- Stehman, S. V. (2014). Estimating area and map accuracy for stratified random sampling when the strata are different from the map classes. *International Journal of Remote Sensing*, 35 (13), 4923-4939.
- Olofsson, P., Foody, G. M., Herold, M., Stehman, S. V., Woodcock, C. E., & Wulder, M. A. (2014). Good practices for estimating area and assessing accuracy of land change. *Remote Sensing of Environment*, 148, 42-57.
