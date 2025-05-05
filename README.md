# JWST PAH Analysis Project
_A Study of Polycyclic Aromatic Hydrocarbons_

---


[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
![Python](https://img.shields.io/badge/python-3.9%2B-blue)

---

## Project Overview

The primary objective of this study is to analyze variations in PAH features across different regions within many galaxies.  
By using high-resolution data from JWST’s MIRI/IFU, we aim to trace changes in PAH size, charge, and composition from the galaxy's nucleus to its outskirts, gaining insights into PAH behavior under diverse galactic conditions.

This project utilizes the MIRI public database to study mid-IR PAH emission in nearby galaxies that exhibit both star-forming activity and active galactic nucleus (AGN) signatures. Our approach examines how the ISM astrochemistry, as revealed by PAH populations, is influenced by the dominant radiation field in each region.

---

## Goals

- Develop a scalable pipeline for PAH analysis across galaxies.
- Integrate the NASA/AMES PAH spectral database (PAHdb) for refined decomposition of PAH sub-populations (size, charge, structure).

---

## Data

- JWST/MIRI IFU spectral cubes (3D and 1D products).
- PAH database from Bauschlicher et al. (2018), Boersma et al. (2014), Mattioda et al. (2020).

---

## Repository Structure

- `1_Polycyclic/` — Data products (JSON, PDF, ECSV)
- `2_Aromatic/` — Jupyter notebooks for PAH analysis and visualization
- `3_Hydrocarbons/` — Processed spectral FITS files

---

## Installation

Clone the repository:
```bash
git clone https://github.com/Astro-cat-mistry/JWSTPAH.git
cd JWSTPAH
pip install -r requirements.txt

## Data Files

The following large JWST MIRI 3D spectral cubes are required for some notebooks.  
Due to GitHub's file size limits, these files are hosted on Google Drive:

| File | Description | Download Link |
|:-----|:------------|:--------------|
| `jw01328-c1006_t014_miri_ch1-shortmediumlong_s3d.fits` | Channel 1 spectral cube | [Download](https://drive.google.com/uc?export=download&id=1-dh21pp5fm88m538zmro95k-o_J65Rsq) |
| `jw01328-c1006_t014_miri_ch2-shortmediumlong_s3d.fits` | Channel 2 spectral cube | [Download](https://drive.google.com/uc?export=download&id=1kn3ZYmedyVoCAvyHbS6iYPcUnMNQH8rK) |
| `jw01328-c1006_t014_miri_ch3-shortmediumlong_s3d.fits` | Channel 3 spectral cube | [Download](https://drive.google.com/uc?export=download&id=1WNcNXjOdLMEKJT_kXz5KXXCqgtDyaBN2) |

👉 Place these files inside the `3_Hydrocarbons/` folder before running the notebooks.
