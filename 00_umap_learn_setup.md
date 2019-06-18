Reference: https://pip.pypa.io/en/stable/installing/#do-i-need-to-install-pip

# Installing python

## Windows

Download and install Git Bash if you have not, using the instructions here

- https://www.youtube.com/watch?v=339AEqk9c-8
- https://carpentries.github.io/workshop-template/ ('The Bash Shell' section)

Follow this link to install Python if you have not. https://www.python.org/ftp/python/3.7.3/python-3.7.3-amd64.exe

1) Run the installer 

2) Uncheck `Install launcher for all users` 

3) Check `Add Python 3.7 to PATH` 

4) Click on `Customize installation`

5) On the `Optional Features` screen, uncheck `for all users (requires elevation)`; leave everything else checked.

6) Click `Next`

7) On the `Advanced Options` screen, only check `Associate...` and `Create...` and `Add...` options.

8) Click `Install`

Once the installer has finished, click on the Start button and search for "Python" - you should see a result for `Python 3.7 (64 bit)`

## Mac

TODO - would a mac person be able to do this?
https://www.python.org/downloads/mac-osx/

# Installing pip package manager

Open a command line prompt and type `pip` then hit enter. If you get usage instructions for `pip`, skip to next section.


If your system does not have `pip`, securely download get-pip.py using a command line prompt:

`$ curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py`

Then run the following:

`python get-pip.py --user`

# UMAP Installation via pip 

```
pip install --upgrade --force-reinstall umap-learn --user
```

### Troubleshooting links:

https://github.com/satijalab/seurat/issues/486
https://github.com/satijalab/seurat/issues/631
https://github.com/satijalab/seurat/issues/1020
https://stackoverflow.com/questions/55975266/reticulate-cant-install-python-packages

https://rstudio.github.io/reticulate/articles/python_packages.html

