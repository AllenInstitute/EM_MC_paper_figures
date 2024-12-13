# EM_MC_paper_figures
Jupyter Notebooks used to analyze and generate figures for "Distinct synaptic connectivity and target specificity of predicted Sst-transcriptomic types in electron microscopy"

## System Requirements
Most Notebooks were run on Python 3.9 on a Windows OS 10 but were tested on Mac OS 14.6.1 and Mac OS ??? and Windows OS 11.
We don't have any reason to believe it would not work on Linux but it has not been tested.
However, Fig2_vtk_render_allcell_outputs_myelin_streamline_for_review was run using Vtk which we were only able to install on Mac OS.

## Environment setup

Clone this repository

```
   git clone git@github.com:AllenInstitute/EM_MC_paper_figures.git
```

Create a python environment and make sure that all the necessary requirements are installed (listed in requirements.txt)
For example setup a new anaconda environemnt or virtual environment then within that environment with Python 3.10 (or Python 3.9 if running the model)


```
   pip install -r requirements.txt 
```
The file includes exact pins in order to reproduce what we did with the paper, though we are not saying that only those versions will work.  You can use requirements.in instead that has no version pins, but use at your own risk as versions might have changed that will break this code.

To run the Classifier_Optimization_And_Met_Predictions.ipynb notebook you need to install a seperate Python 3.6 environment

```
   conda create -n EM_MC_paper_figs_py36_10 python=3.6.10
   conda activate EM_MC_paper_figs_py36_10
   conda install ipykernel
   pip -r requirementspy36.txt
```

## Data download
The mm3 EM dataset is publicly available at: https://www.microns-explorer.org/cortical-mm3. Analysis for this paper was performed on version 661 of the dataset, a snapshot taken on September 19th, 2023 at 4:00am UTC.

The Patch-seq gene expression data “Mouse Patchseq VIS - RNAseq” is publicly available at: https://knowledge.brain-map.org/data/1HEYEW7GMUKWIQW37BO/
Summary and the associated cell metadata is available here: https://portal.brain-map.org/cell-types/classes/multimodal-characterization. 

## Level of support
We are not currently supporting this code, but simply releasing it to the community AS IS but are not able to provide any guarantees of support. The community is welcome to submit issues, but you should not expect an active response.
