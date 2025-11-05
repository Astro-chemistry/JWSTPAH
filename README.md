# JWST PAH Analysis Project
*Mapping the size, charge, and structure of PAHs in nearby galaxies using JWST/MIRI.*

![Python](https://img.shields.io/badge/python-3.9%2B-blue)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

---

## Description

This repository contains analysis workflows and exploratory notebooks used to study
polycyclic aromatic hydrocarbons (PAHs) in JWST/MIRI IFU data.

The scientific goal is to examine how PAH populations (size, ionization state, and molecular structure)
vary from the AGN-dominated centers of galaxies to their star-forming outskirts.

---

## Repository Layout


JWSTPAH/
├─ Whole pipeline.ipynb # Complete end-to-end workflow (main run notebook)
├─ Extraction.ipynb # Notes and tests for annular spectrum extraction
├─ Stitching.ipynb # Channel stitching development and validation
├─ PAH-fit-database.ipynb # Experiments using PAHFIT and PAHdb

└─ previous_versions/ # Older exploratory notebooks kept for reference
├─ 1.0.ipynb
├─ 1.1.ipynb
├─ 2.0.ipynb
├─ 2.1.ipynb
└─ 2.2.ipynb


### Large Data
FITS cubes **are not stored in this repository**.
Store them locally and update paths inside notebooks accordingly.

---

## Installation

```bash
conda create -n jwstpah python=3.11
conda activate jwstpah
pip install -r requirements.txt
jupyter lab
Data Setup

Expected local structure:

data/
└─ raw/
   └─ NGC7469/
      ├─ jw01328_c1006_ch1_s3d.fits
      ├─ jw01328_c1006_ch2_s3d.fits
      └─ jw01328_c1006_ch3_s3d.fits

Citation

If you use this repository or derive results from it in academic work, please cite:

Maldonado-Portilla, Juan José et al.,
PAH Emission Mapping with JWST/MIRI,
in preparation (2025).
DOI / arXiv link will be added upon publication.

See CITATION.cff
 for formal citation metadata.
GitHub will display a “Cite this repository” button automatically.

License

This project is open-source under the MIT License (with citation notice).
See LICENSE
.
