# UCSF DSI scRNA seq

Welcome to the UCSF Data Science Initiative's single-cell RNA-sequencing workshop. This course is built from the following Satija Lab Seurat vignettes:

- [Guided Clustering with Seurat](https://satijalab.org/seurat/v3.0/pbmc3k_tutorial.html)

- [Integrating Stimulated vs. Control PBMC datasets](https://satijalab.org/seurat/v3.0/immune_alignment.html)

We add emphasis to areas of the vignettes we find most important, expand explanations in key areas, and add some of our own data processing and analysis if needed.

### Official UCSF DSI Course Materials

Team-reviewed, tested, and ready-to-use materials will always be hosted on our official UCSF Collaborative Learning Environment (CLE) [scRNA-seq webpage](https://courses.ucsf.edu/course/view.php?id=6154).

_This GitHub repository is for development purposes and therefore may stray from the materials used in class._ CLE will remain as it was at the time of our most recently offered workshop and will only be updated if major changes are introduced to the course.

Branch "master" should function as intended if cloned, but for verified materials please download all documents and data from CLE unless otherwise instructed.

# Workshop Setup Instructions:

#### *Please do not wait until the day of the workshop to do these installations*! We cannot spend class time working through installation issues.

In order to install and use the R packages required for this workshop, you must also have the following installed on your system:

1. Python
2. pip
3. UMAP
4. R Packages

Instructions for each are below. If you have trouble with installations up until the day before the workshop, please email both Angelo and Karla:  

- Angelo Pelonero: [angelo.pelonero@ucsf.edu](mailto:angelo.pelonero@ucsf.edu)

- Karla Lindquist: [karla.lindquist@ucsf.edu](mailto:karla.lindquist@ucsf.edu)  

Instructors will also be in the classroom half an hour before a workshop begins. However, this time will be for minor troubleshooting issues only. If you have major issues (or if you wait until this time to begin your installations) we cannot guarantee that you will be set up in time to follow along with the workshop.     

## Installing python:

#### Windows users

Download and install Git Bash if you have not, using the instructions here

- [https://www.youtube.com/watch?v=339AEqk9c-8](https://www.youtube.com/watch?v=339AEqk9c-8)
- [https://carpentries.github.io/workshop-template/](https://carpentries.github.io/workshop-template/) ('The Bash Shell' section)

Follow this link to install Python if you have not: [https://www.python.org/ftp/python/3.7.3/python-3.7.3-amd64.exe](https://www.python.org/ftp/python/3.7.3/python-3.7.3-amd64.exe)

1. Run the installer 

2. Uncheck `Install launcher for all users` 

3. Check `Add Python 3.7 to PATH` 

4. Click on `Customize installation`

5. On the `Optional Features` screen, uncheck `for all users (requires elevation)`; leave everything else checked.

6. Click `Next`

7. On the `Advanced Options` screen, only check `Associate...` and `Create...` and `Add...` options.

8. Click `Install`

Once the installer has finished, click on the Start button and search for "Python" - you should see a result for `Python 3.7 (64 bit)`

#### Mac users

Python 3.7 installation files are can be found here: [https://www.python.org/downloads/release/python-373/](https://www.python.org/downloads/release/python-373/)

If you are working on a 64-bit Mac OS X 10.9 or later system, please download the "macOS 64-bit installer" file, then double click on it and follow the installation instructions.

For those working on 32-bit or 64-bit Mac OS X 10.6 to 10.8 systems, please download the "macOS 64-bit/32-bit installer" file, then double click on it and follow the installation instructions.


## Installing pip:

Reference: [https://pip.pypa.io/en/stable/installing/#do-i-need-to-install-pip](https://pip.pypa.io/en/stable/installing/#do-i-need-to-install-pip)

To check if you have pip installed:

1. Open a terminal/command line prompt and type `pip` then hit enter. If you get usage instructions for `pip`, skip to next section (Installing UMAP).


2. If your system does not have `pip`, securely download get-pip.py using a command line prompt:

`$ curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py`

3. Then run the following:

`python get-pip.py --user`


## Installing UMAP:

`pip install --upgrade --force-reinstall umap-learn --user`

## Installing R Packages:
We package R installations in .Rmd format - you'll need to have [R](https://www.r-project.org) and [RStudio](https://www.rstudio.com/products/rstudio/download/) installed to proceed.

Open `0_workshop_prep.Rmd` in Rstudio, run all the cells, and ensure all packages install without issue. Once done, you're ready for the workshop. And remember, please contact us ASAP if you have any trouble!

###### Troubleshooting links:

[https://github.com/satijalab/seurat/issues/486](https://github.com/satijalab/seurat/issues/486)

[https://github.com/satijalab/seurat/issues/631](https://github.com/satijalab/seurat/issues/631)

[https://github.com/satijalab/seurat/issues/1020](https://github.com/satijalab/seurat/issues/1020)

### Update readme with new setup instructions (no reticulate)

[https://stackoverflow.com/questions/55975266/reticulate-cant-install-python-packages](ttps://stackoverflow.com/questions/55975266/reticulate-cant-install-python-packages)

[https://rstudio.github.io/reticulate/articles/python_packages.html](https://rstudio.github.io/reticulate/articles/python_packages.html)

# About scRNA-seq data preprocessing:
This workshop outlines the general workflow for analysis of scRNA seq data that that has already been preprocessed into either 10x Genomics' CellRanger output (.Rmd #s 1-5) or count matrices (.Rmd # 6).

The majority of this workshop (notebooks 1-5) uses data output from the 10x Genomics CellRanger Pipeline. This software can demultiplexes, counts, and aggregates raw basecall data directly from Illumina sequencers:

![General scRNAseq workflow](https://support.10xgenomics.com/img/cellranger-workflows/cellranger_simplest_1_bw_2.png)
######Source: 10x Genomics

__Please note that this pipeline is not necessary for this workshop__ but will be needed to use your data with these notebooks. Visit the [10x Genomics CellRanger Pipeline website](https://support.10xgenomics.com/single-cell-gene-expression/software/pipelines/latest/what-is-cell-ranger) for installation instructions, user guides, and more information.

# About Seurat:

Seurat is an R toolkit for single cell genomics, developed and maintained by the Satija Lab at NYGC. Instructions, documentation, version history, and additional tutorials can be found on the [Satija Lab Webpage](https://satijalab.org/seurat). Seurat is also hosted on the Satija Lab GitHub, you can view and clone the repository [here](https://github.com/satijalab/seurat).

Seurat has been successfully installed on Mac OS X, Linux, and Windows, using the devtools package to install directly from GitHub. Improvements and new features will be added to the Satija Lab GitHub on a regular basis, please contact seuratpackage@gmail.com with any questions or if you would like to contribute.

# GitHub and UCSF data security protocols:

Please be aware that **GitHub is not certified for use with personal health information (PHI).** Do not store or share any sensitive information via GitHub, even if kept in private repositories.

For more information regarding UCSF's security guidelines, [please see the UCSF IRB guidelines for electronic data security.](https://irb.ucsf.edu/electronic-data-security)
