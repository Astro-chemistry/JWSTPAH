# JWST PAH Analysis Project

Analysis of polycyclic aromatic hydrocarbons (PAHs) in galaxies observed with JWST/MIRI IFU. This repository contains notebooks for extracting radial annular spectra, stitching spectral channels, and testing PAHFIT/PAHdb decomposition to study PAH size, ionization, and structure variations from galaxy nuclei toward star-forming regions.

## Repository Contents

Whole pipeline.ipynb — current end-to-end workflow  
Extraction.ipynb — extraction tests and notes  
Stitching.ipynb — channel stitching tests and validation  
PAH-fit-database.ipynb — PAHFIT / PAHdb exploration  

previous_versions/ — archived exploration notebooks  
(1.0.ipynb, 1.1.ipynb, 2.0.ipynb, 2.1.ipynb, 2.2.ipynb)

Large FITS data products are not stored in this repository. They should be kept locally.

## Environment Setup

conda create -n jwstpah python=3.11  
conda activate jwstpah  
pip install -r requirements.txt  
jupyter lab

## Local Data Structure

data/raw/NGC7469/ should contain the CH1, CH2, and CH3 JWST/MIRI IFU cubes.

## Citation

If you use this repository or any part of its workflow in scientific work, please cite:

Maldonado-Portilla, Juan José et al.  
"PAH Emission Mapping with JWST/MIRI"  
In preparation (2025). DOI/arXiv will be added.

Citation metadata is provided in CITATION.cff (GitHub will display “Cite this repository”).

## License

MIT License with citation notice. See LICENSE for details.
