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

(State one or more sections that will comprise the notebook. E.g., _This cookbook is broken up into two main sections - "Foundations" and "Example Workflows."_ Then, describe each section below.)

### Section 1 ( Replace with the title of this section, e.g. "Foundations" )

(Add content for this section, e.g., "The foundational content includes ... ")

### Section 2 ( Replace with the title of this section, e.g. "Example workflows" )

(Add content for this section, e.g., "Example workflows include ... ")

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

(Replace "cookbook-example" with the title of your cookbooks)

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
