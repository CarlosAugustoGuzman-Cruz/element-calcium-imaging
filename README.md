# DataJoint Workflow - Calcium Imaging

Workflow for calcium imaging data acquired with 
[ScanImage](http://scanimage.vidriotechnologies.com),  
[Scanbox](https://scanbox.org), or `Nikon NIS` software and processed with 
[Suite2p](https://github.com/MouseLand/suite2p) or 
[CaImAn](https://github.com/flatironinstitute/CaImAn).

A complete calcium imaging workflow can be built using the DataJoint Elements.
+ [element-lab](https://github.com/datajoint/element-lab)
+ [element-animal](https://github.com/datajoint/element-animal)
+ [element-session](https://github.com/datajoint/element-session)
+ [element-calcium-imaging](https://github.com/datajoint/element-calcium-imaging)

This repository provides demonstrations for:
1. Set up a workflow using DataJoint Elements (see 
[workflow_calcium_imaging/pipeline.py](workflow_calcium_imaging/pipeline.py))
2. Ingestion of data/metadata based on a predefined file structure, file naming 
convention, and directory lookup methods (see 
[workflow_calcium_imaging/paths.py](workflow_calcium_imaging/paths.py)).
3. Ingestion of segmentation and deconvolution results.

## Workflow architecture

The calcium imaging workflow presented here uses components from four DataJoint 
Elements ([element-lab](https://github.com/datajoint/element-lab), 
[element-animal](https://github.com/datajoint/element-animal), 
[element-session](https://github.com/datajoint/element-session), 
[element-calcium-imaging](https://github.com/datajoint/element-calcium-imaging)) 
assembled together to form a fully functional workflow. 

![element_calcium_imaging](images/attached_calcium_imaging_element.svg)

## Installation instructions

+ The installation instructions can be found at 
[datajoint-elements/install.md](
     https://github.com/datajoint/datajoint-elements/blob/main/gh-pages/docs/usage/install.md).

## Interacting with the DataJoint workflow

+ Please refer to the following workflow-specific 
[Jupyter notebooks](/notebooks) for an in-depth explanation of how to run the 
workflow ([03-process.ipynb](notebooks/03-process.ipynb)) and explore the data 
([05-explore.ipynb](notebooks/05-explore.ipynb)).
