# ITA PhD course

*Computational research with COMPAS*

## Description

The PhD-level course (primarily for A&T PhDs) will introduce computational methods for architecture engineering, fabrication & construction, incentivising computational literacy. Students learn the theoretical background and basic implementation details of fundamental data structures and algorithms, and to solve real-world problems using the COMPAS framework and other open-source libraries.

## Learning objectives

* understand the scope and relevance of computational methods for architecture and engineering research and practice,
* the theoretical background of fundamental data structures,
* the basic principles of algorithmic design;
* implement basic versions of prevalent algorithms related to architectural geometry, structural design, robotic assembly, volumetric modeling & 3D-printing, high-performance computation;
* use sophisticated algorithms available through open-source libraries to solve real-world problems; and,
* use common CAD tools as interfaces to self-implemented solutions.

## Overview

Course will consist of a few lectures, several tutorials and project-based exercises.

Topics will include:

* Intro Python programming
* Intro COMPAS open-source framework (https://compas-dev.github.io/)
* Intro to geometry processing, data structures, topology, numerical computation
* Domain-specific case studies (e.g. on architectural geometry, structural design, robotic assembly, volumetric modeling and 3D printing, high performance computation)

## Schedule

Week | Date | Lead | Title | Description | Links
---- | ---- | ---- | ----- | ----------- | -------
1 | Oct 2 | BRG | Introduction | Course overview, COMPAS intro | [Slides](slides/week-01_COMPAS-basics.pdf)
2 | Oct 9 | GKR | Getting Started | Development Tools 101<br>Python 101<br>COMPAS 101 | [Slides](slides/week-02_Getting_started.pdf), [Assignment](modules/module0/01_getting_started/README.md)
3 | Oct 23 | BRG | Data structures and Geometry | Basic theory and examples | [Slides](slides/week-03_Geometry-and-Data-Structures.pdf), [Assignment](modules/module0/02_datastructures_and_geometry/README.md)
4 | Oct 30 | BRG | Module 1: Structural Design | **Theory:** Form Finding methods | [Slides](slides/week-4_Structural-Design.pdf), [Assignment](modules/module1/assignments/README.md)
5 | Nov 6 | BRG | Module 1: Structural Design | **Case study:** The HiLo cablenet formwork system | [Slides](slides/week-5_Structural-Design.pdf)
6 | Nov 13 | GKR | Module 2: Robotic Assembly | **Theory:** Robotic fabrication planning and executing | [Slides](https://docs.google.com/presentation/d/1OIU3vCmwe3lkVWpI0JuJJ-GFoOq5HH8ulElPZNS_F2Y/edit?usp=sharing), [Jupyter Notebook](modules/module2/Frame%20and%20Transformation.ipynb), [Assignment](modules/module2/assignments/session1.md)
7 | Nov 20 | GKR | Module 2: Robotic Assembly | **Case study:** Robotic assembly of a brick wall | [Slides](https://docs.google.com/presentation/d/1S29aMP9h4nRvQCdr1jGvp0L4YQCc8q0_irpHb9p9kos/edit?usp=sharing), [Assignment](modules/module2/assignments/session2.md)
8 | Nov 27 | DBT | Module 3: Volumetric Modeling | **Theory:** Modelling with signed distance functions | [Slides](slides/week-08_VolumetricModelling.pdf), [Notebooks](modules/module3/week1), [Assignment](modules/module3/week1/Assignment/README.md)
9 | Dec 4 | DBT | Module 3: Volumetric Modeling | **Case study:** Modelling of a node | [Slides](slides/week-09_VolumetricModelling_2.pdf), [Notebooks](modules/module3/week2), [Assignment](modules/module3/week2/Assignment/README.md)
10 | Dec 11 | BRG | Next Steps | Using COMPAS in your own work

## Join us on slack

https://tinyurl.com/yxse82a7

## Jupyter and extensions

Make sure you install `jupyter` and extensions in the environment you are using:

    conda install jupyter jupyter_contrib_nbextensions jupyter_nbextensions_configurator rise pythreejs --yes

To run the jupyter notebook, you simply have to type:

    jupyter notebook

in your command line.

### Activating extensions

From the `Nbextensions` tab in the notebook, install the following extensions:

1. Split Cells Notebook: Enable split cells in Jupyter notebooks
2. RISE: allows you to instantly turn your Jupyter Notebooks into a slideshow.

### Configure workspace

To configure the workspace, type

    jupyter notebook --generate-config

This writes a default configuration file into:

`%HOMEPATH%\.jupyter\jupyter_notebook_config.py` (on windows)

or

`~/.jupyter/jupyter_notebook_config.py` (on mac)

If you want jupyter to open in a different directory, then change the following line:

    c.NotebookApp.notebook_dir = 'YOUR_PREFERRED_PATH'
