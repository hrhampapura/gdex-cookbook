# GDEX Cookbook

<img src="thumbnails/gdex_logo.png" alt="thumbnail" width="300"/>

[![nightly-build](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/cookbook-template/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/475509405.svg)](https://zenodo.org/badge/latestdoi/475509405)

This Project Pythia Cookbook covers what data users and submitters need to know about NSF NCAR's Geoscience Data Exchange (GDEX), a major geoscience data repository.

## Motivation

NSF NCAR's Geoscience Data Exchange (GDEX) hosts thousands of freely accessible geoscience datasets — from global reanalyses like ERA5 and JRA-3Q to climate model output and observational records — but knowing how to find, access, and work with that data can be a significant barrier for new users. This cookbook removes that barrier. By the end, you will know how to discover datasets on GDEX, choose the right access method for your workflow (bulk download, THREDDS/OPeNDAP streaming, Zarr cloud access, Globus, or the REST API), and apply those skills to real datasets across a range of geoscience workflows. You will also learn how to submit your own data to GDEX for long-term stewardship and citation.

## Authors

[Harsha R. Hampapura](https://github.com/hrhampapura)
[Riley Conroy](https://github.com/rpconroy)
[Chia-Wei Hsu](https://github.com/chiaweh2)
[Mya Sears](https://github.com/myasea8)

### Contributors

<a href="https://github.com/ProjectPythia/gdex-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/gdex-cookbook" />
</a>

## Structure

This cookbook is organized into three main sections — **GDEX Introduction**,
**Services**, and **Example Workflows** — building from orientation, to access
methods, to complete analyses.

### GDEX Introduction

A high-level tour of what GDEX is and who it serves: what the repository holds, the
services it offers for accessing and contributing data, how it enables science, and
how to submit your own datasets.

### Services

The core access toolkit — each subsection covers one way to get data out of GDEX,
with a short introduction plus hands-on notebooks:

- **TDS** — the THREDDS Data Server: OPeNDAP and remote subsetting via xarray and Siphon
- **Zarr/Kerchunk** — Analysis-Ready, Cloud-Optimized access to virtual Zarr stores
- **API** — programmatic dataset discovery, metadata, and subsetting
- **Direct Download** — pulling files over HTTPS
- **POSIX** — direct filesystem access on NSF NCAR HPC
- **Globus** — high-performance transfer of large datasets

### Example Workflows

End-to-end, dataset-specific analyses that put those services to work — each streams
data remotely (no bulk downloads) and produces a diagnostic or visualization:

- **Reanalysis** — ERA5 precipitation and JRA-3Q sea-level pressure
- **Model Simulations** — CESM2 Large Ensemble, NA-CORDEX, and CONUS404
- **Observations** — HadISST sea surface temperature and S-Pol radar
- **Data Fusion** — combining wind-profiler observations with ERA5

## Running the Notebooks

You can either run the notebooks in the Cookbook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables "one click"
execution in the cloud. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon (see screenshots [here](https://foundations.projectpythia.org/preamble/how-to-use/#running-pythia-foundations-examples)),
and a text box will appear. Type or paste the Pythia Binder link
(`https://binder.projectpythia.org`) and click "Launch".
After a few moments you should be presented with a
notebook that you can interact with. You’ll be able to execute code
and even change the example programs. At first the code cells
have no output, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in the Pythia Foundations chapter [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter).

Note, not all Cookbook chapters are executable. If you do not see
the rocket ship icon, such as on this page, you are not viewing an
executable book chapter.


### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/ProjectPythia/gdex-cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/gdex-cookbook.git
   ```

1. Move into the `gdex-cookbook` directory
   ```bash
   cd gdex-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate gdex-cookbook
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
