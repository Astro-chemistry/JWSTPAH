# SHIRO: Spectral Homogenization, Infrared Radial Output

SHIRO is a JWST/MIRI MRS analysis pipeline for spatially resolved studies of polycyclic aromatic hydrocarbon (PAH) emission in galaxies.

Developed and tested using observations of NGC 7469, the pipeline provides an end-to-end workflow for extracting annular spectra, stitching MIRI spectral channels, performing PAHFIT decomposition, propagating uncertainties through Monte Carlo simulations, and analyzing PAH populations using PAHdb.

## Pipeline Overview

The notebook performs the following steps:

1. Discovery and loading of MIRI/MRS spectral cubes
2. Spatial homogenization through PSF matching
3. Quality-assurance maps with annular overlays
4. Annular spectral extraction
5. Pre-stitch spectral diagnostics
6. Spectral stitching across sub-bands and channels
7. Spectral decomposition with PAHFIT
8. Extraction of PAH-only spectra
9. Monte Carlo uncertainty estimation
10. PAH band-ratio measurements with propagated uncertainties
11. Radial trend analysis
12. PAH population analysis using PAHdb

## Repository Contents

* `SHIRO - Spectral Homogenization, Infrared Radial Output.ipynb`

  Complete end-to-end analysis pipeline.

## Using the Pipeline for Other Galaxies

To adapt the workflow to a new target:

* Set `galaxy_folder` to the directory containing the JWST/MIRI `_s3d.fits` cubes.
* Update `REDSHIFT` to the target galaxy value.
* Adjust the annular extraction parameters (`num_rings`, `r0`, and `step`) as needed.
* Verify that the PAHFIT feature names in `BAND_COMPLEXES` match those produced by PAHFIT for the target.

## External Data Requirements

This repository does not distribute JWST data products or PAHdb databases.

### JWST Data

Users must provide their own JWST/MIRI MRS `_s3d.fits` cubes.

### PAHdb

PAHdb files must be downloaded separately and placed in a local `PAHdb/` directory.

The databases are not distributed through this repository because of their size.

## Scientific Improvements Relative to Earlier Versions

* Consistent redshift handling throughout the workflow
* Science-ready PSF homogenization
* Monte Carlo uncertainty propagation
* PAH band-ratio uncertainties included in final plots
* Improved robustness in PAHFIT feature extraction

## Citation

If you use SHIRO in academic work, please cite the repository using the metadata provided in `CITATION.cff`.

GitHub will automatically generate citation formats through the repository's **Cite this repository** feature.

## Acknowledgments

Developed at the Observatório do Valongo, Universidade Federal do Rio de Janeiro (UFRJ).

Advisor: Karín Menéndez-Delmestre

Author: Juan José Maldonado-Portilla

## License

MIT License. See `LICENSE` for details.
