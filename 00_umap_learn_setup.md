Reference: https://pip.pypa.io/en/stable/installing/#do-i-need-to-install-pip

# Installing pip package manager

To install pip, securely download get-pip.py. [1]:

`$ curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py`

Then run the following:

`python get-pip.py --user`

# UMAP Installation via pip 

```
pip install --upgrade --force-reinstall umap-learn --user
```

## TODO
Will using --user allow RStudio to find the umap package? Currently not working on windows, not sure why.