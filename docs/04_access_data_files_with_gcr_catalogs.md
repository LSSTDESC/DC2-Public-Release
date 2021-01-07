# Access Data Files with GCRCatalogs


After you [downloaded the data files](01_download_data_files.md) and [installed `GCRCatalogs`](03_install_gcr_catalogs.md),
you need to tell `GCRCatalogs` where these downloaded files sit on your machine. 

When you used Globus transfer, if you downloaded the files to `/path/to/the/download/directory`, then run in a terminal

```bash
python -m GCRCatalogs.user_config set root_dir /path/to/the/download/directory
```

Here `/path/to/the/download/directory` should contain the `lsstdesc-public` folder that Globus transfer creates. 
If you have moved it, you should change `/path/to/the/download/directory` to the directory that contains the `lsstdesc-public` folder.
Do not change the directory structure within `lsstdesc-public`. 

You only need to set this once. 
