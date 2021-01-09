## Install and Configure GCRCatalogs

You can install [`GCRCatalogs`](https://github.com/LSSTDESC/gcr-catalogs) with [conda](https://docs.conda.io/) or [pip](https://pip.pypa.io/),
depending on your local Python environment.

### Install with conda

You may want to create a new conda environment before installation.
If you do, [see instructions here](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).

To install, simply run

```bash
conda install lsstdesc-gcr-catalogs -c conda-forge/label/lsstdesc-gcr-catalogs_rc
```

### Install with pip

You may want to create a virtual environment before installation.
If you do, [see instructions here](https://docs.python.org/3/library/venv.html).

To install, simply run

```bash
pip install https://github.com/LSSTDESC/gcr-catalogs/archive/v1.2.0rc2.tar.gz#egg=GCRCatalogs[full]
```

### Configure: Setting up `root_dir` for GCRCatalogs

After you [downloaded the data files](01_download_data_files.md) and [installed `GCRCatalogs`](03_install_gcr_catalogs.md),
you need to tell `GCRCatalogs` where these downloaded files sit on your machine. 

When you used Globus transfer, if you downloaded the files to `/path/to/the/download/directory`, then run in a terminal

```bash
python -m GCRCatalogs.user_config set root_dir /path/to/the/download/directory
```

Here `/path/to/the/download/directory` should contain the `lsstdesc-public` folder that Globus transfer creates. 
If you have moved this folder, you should change `/path/to/the/download/directory` to the directory that now contains it.
Do not change the directory structure within `lsstdesc-public`. 

You only need to issue this command once. 

