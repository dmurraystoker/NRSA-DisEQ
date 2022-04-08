# NRSA-DisEQ

Data, code, and metadata for the manuscript:

Murray-Stoker, David, Kelly M. Murray-Stoker, Fan Peng Kong, and Fathima Amanat. Environmental filtering and habitat (mis)matching of riverine invertebrate metacommunities.


[![DOI](https://zenodo.org/badge/476883723.svg)](https://zenodo.org/badge/latestdoi/476883723)


## Abstract

**Aim:** Metacommunities are assembled through a combination of local and regional processes, with the relative importance of the drivers of assembly depending on ecological context. Global change can alter community assembly at both local and regional levels, potentially shifting communities into disequilibrium with their local environmental conditions. In this study, we evaluated the spatial variation in environmental filtering and habitat matching of 1078 riverine macroinvertebrate communities distributed across nine ecoregions within the conterminous United States.

**Location:** Conterminous United States.

**Taxon:** Freshwater macroinvertebrates.

**Methods:** We first quantified spatial patterns in environmental filtering, habitat matching, and functional trait diversity. We then used boosted regression trees to identify (1) functional trait predictors of environmental filtering and habitat match and (2) environmental, landscape, and network variables that predict functional trait abundances. 

**Results:** Our results demonstrated that environmental filtering but not habitat matching varied strongly by ecoregion. We also found that functional trait diversity varied by ecoregion, but not as strongly as the signatures of environmental filtering. We did not identify consistent functional trait predictors for both environmental filtering and habitat matching, with trait predictors instead varying by individual traits, trait categories, and ecoregions. Notwithstanding inconsistent trait predictors, environmental filtering was primarily influenced by habitat preference traits while habitat matching was primarily influenced by both habitat preference and dispersal traits. Predictors of functional traits also varied by trait category and ecoregion, with habitat preference and dispersal traits primarily influenced by network variables.

**Main conclusions:** Our study demonstrates the contingent patterns and drivers of environmental filtering and habitat matching on a macroecological scale. We aim for this work to provide the foundation on which trait-environment relationships can be further quantified and causal explanations established in the context of community disequilibrium and applied to conservation and management of freshwater systems.
Keywords: community disequilibrium, freshwater ecology, functional traits, global change, macroecology, metacommunity ecology, trait-environment relationships


## Contents

The [R Project](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/NRSA-DisEQ.Rproj) provides a local relative directory for all data and code.


### Data

All processed data are provided in the [data folder](https://github.com/dmurraystoker/NRSA-DisEQ/tree/main/data), Metadata are provided [here](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/metadata.md).


### R Code & Data Analysis Summary Reports

All analytical code and summary reports are provided in the [data analysis folder](https://github.com/dmurraystoker/NRSA-DisEQ/tree/main/data_analysis). We also provide summary reports to aid in the evaluation of results, with code chunks echoing the data management and analyses

We first processed the raw invertebrate data into a workable dataset using the [0-data_management.Rmd](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/0-data_management/0-data_management.Rmd). 

Second, we put the data through the DisEQ pipeline, described by [Blonder et al. (2015)](http://doi.wiley.com/10.1890/14-0589.1). We provide the [1-DisEQ_pipeline.Rmd](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/1-DisEQ_pipeline/1-DisEQ_pipeline.Rmd) code to run the pipeline and merging environmental, landscape, and network predictor variables. We provide the DisEQ pipeline workspace [1-DisEQ_pipeline-DisEQ_data.RData](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/1-DisEQ_pipeline/1-DisEQ_pipeline.Rmd), which was used for downstream analyses.

Third, we provide the focal code for conducting statistical analyses in the [2-DisEQ_analyses.Rmd](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/2-DisEQ_analyses/2-DisEQ_analyses.Rmd) script, where the [1-DisEQ_pipeline-DisEQ_data.RData](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/1-DisEQ_pipeline/1-DisEQ_pipeline.Rmd) workspace was loaded for further analyses. From the DisEQ analyses, we exported a reduced workspace [2-DisEQ_analyses-Reduced_Workspace.RData](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/2-DisEQ_analyses/2-DisEQ_analyses-Reduced_Workspace.RData). The full workspace included all boosted regression tree objects, which results in a very large workspace (> 1.5 GB), while the reduced workspace contains the relative influence summaries as they were most important for interpreting the results. The full workspace can be generated by running the entire script, including the boosted regression trees. Alternatively, you can contact me via electronic mail (David Murray-Stoker, dstoker92@gmail.com) and we can find the most accessible way to download the workspace.

We provide all the code for figure creation in the [3-figures.Rmd](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/3-figures/3-figures.Rmd) file, with final edits to figures done in Adobe Illustrator.

Lastly, we provide [summary tables of the boosted regression trees](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/4-supplementary_BRT_results/4-supplementary_BRT_results.pdf) and [environmental, landscape, and network predictor variable summaries](https://github.com/dmurraystoker/NRSA-DisEQ/blob/main/data_analysis/5-supplementary_variable_summaries/5-supplementary_variable_summaries.pdf). Both sets of summary tables are used to supplement results.


## Using the Repository

To use the data and R code for this project:

1. `git clone` this repository or download it as a zip folder

2. Open `R Studio`, go to `file > Open project` and open the `NRSA-DisEQ.Rproj` R Project associated with this repository

3. Analyses can be done using code in the [data analysis folder](https://github.com/dmurraystoker/OGC-biomass/tree/main/data_analysis)






