# 🌌WS JWST PAH Analysis Project
_A Study of Polycyclic Aromatic Hydrocarbons in NGC 7469_

---


![License](https://img.shields.io/github/license/Astro-cat-mistry/JWSTPAH)
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
