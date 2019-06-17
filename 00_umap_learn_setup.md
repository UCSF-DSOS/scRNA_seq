# pip installation for UMAP

Reference: https://pip.pypa.io/en/stable/installing/#do-i-need-to-install-pip

## Installing with get-pip.py
To install pip, securely download get-pip.py. [1]:

`$ curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py`

Then run the following:

`python get-pip.py --user`

## Upgrading pip
On Linux or macOS:

`pip install -U pip`

On Windows:

`python -m pip install -U pip --user`

## Install umap-learn

`$ pip install umap-learn --user`

## TODO
Will using --user allow RStudio to find the umap package? Currently not working on windows.