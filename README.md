# UCSF DSI scRNA seq

Welcome to the UCSF Data Science Initiative's single-cell RNA-sequencing workshop development repo. The content found here is subject to frequent change - if you are looking for versions of these notebooks that were used in workshops, they can be found on their respective course pages. You can also browse commits in this repo - workshop release versions will be flagged with "MM/DD/YY workshop content" for reference.

 This workshop is built primarily atop the following Satija Lab Seurat vignettes:

Guided Clustering with Seurat:
*https://satijalab.org/seurat/v3.0/pbmc3k_tutorial.html

Integrating Stimulated vs. Control PBMC datasets:
*https://satijalab.org/seurat/v3.0/immune_alignment.html

We add emphasis to areas of the vignettes we find most important, expand explanations in key areas, and add some of our own data processing and analysis if needed.

## About Seurat:

Seurat is an R toolkit for single cell genomics, developed and maintained by the Satija Lab at NYGC.

Instructions, documentation, and tutorials can be found at:
* https://satijalab.org/seurat

Seurat is also hosted on GitHub, you can view and clone the repository at
* https://github.com/satijalab/seurat

Seurat has been successfully installed on Mac OS X, Linux, and Windows, using the devtools package to install directly from GitHub

Improvements and new features will be added on a regular basis, please contact seuratpackage@gmail.com with any questions or if you would like to contribute

For more information, vignettes. and version history, see:
*https://satijalab.org/seurat/

DEV TODO:

- Add examples to read in multiple data sources
- Add check for doublets
- Clean up cluster identities in .Rmd #6
- Clarify complicated procedures in .Rmd #s 4, 5, 6 if necessary