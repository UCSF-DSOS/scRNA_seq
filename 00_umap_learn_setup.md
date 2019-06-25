In order to install and use the R packages required for this workshop, you must also have the following installed on your system:

1. Python
2. pip
3. UMAP

Instructions for each are below.  
### *Please do not wait until the day of the workshop to do these installations*! We will not be spending any class time working on installation issues.  

If you have trouble with installations up until the day before the workshop, please email both Angelo and Karla:  
Angelo Pelonero: angelo.pelonero@ucsf.edu  
Karla Lindquist: karla.lindquist@ucsf.edu  

We will also be in the classroom half an hour before the workshop begins. However, this time will be for minor troubleshooting issues only. If you have major issues, or if you wait until this time to begin your installations, we cannot guarantee that you will be set up in time to follow along with the workshop.      

	Installing python

## Windows users

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

## Mac users

Python 3.7 installation files are can be found here: [https://www.python.org/downloads/release/python-373/](https://www.python.org/downloads/release/python-373/)

If you are working on a 64-bit Mac OS X 10.9 or later system, please download the "macOS 64-bit installer" file, then double click on it and follow the installation instructions.

For those working on 32-bit or 64-bit Mac OS X 10.6 to 10.8 systems, please download the "macOS 64-bit/32-bit installer" file, then double click on it and follow the installation instructions.


	Installing pip

Reference: [https://pip.pypa.io/en/stable/installing/#do-i-need-to-install-pip](https://pip.pypa.io/en/stable/installing/#do-i-need-to-install-pip)

To check if you have pip installed:

1. Open a terminal/command line prompt and type `pip` then hit enter. If you get usage instructions for `pip`, skip to next section (Installing UMAP).


2. If your system does not have `pip`, securely download get-pip.py using a command line prompt:

`$ curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py`

3. Then run the following:

`python get-pip.py --user`


	Installing UMAP 

`pip install --upgrade --force-reinstall umap-learn --user`


	Troubleshooting links:

[https://github.com/satijalab/seurat/issues/486](https://github.com/satijalab/seurat/issues/486)
[https://github.com/satijalab/seurat/issues/631](https://github.com/satijalab/seurat/issues/631)
[https://github.com/satijalab/seurat/issues/1020](https://github.com/satijalab/seurat/issues/1020)
[https://stackoverflow.com/questions/55975266/reticulate-cant-install-python-packages](ttps://stackoverflow.com/questions/55975266/reticulate-cant-install-python-packages)
[https://rstudio.github.io/reticulate/articles/python_packages.html](https://rstudio.github.io/reticulate/articles/python_packages.html)

