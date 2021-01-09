## Access Data Files with GCRCatalogs


### Checking that everything is ready

You can use the following Python code to check if you have `GCRCatalogs` installed and `root_dir` correctly set.
The lower two lines should print out the tracts that you have downloaded for Object and Truth tables, respectively.

```python
import GCRCatalogs
print(GCRCatalogs.load_catalog('desc_dc2_run2.2i_dr6_object').available_tracts)
print(GCRCatalogs.load_catalog('desc_dc2_run2.2i_dr6_truth').available_tracts)
```

### Following the notebooks to access data

You can find examples of using `GCRCatalogs` in our [tutorial notebooks](https://github.com/LSSTDESC/DC2-Public-Release/tree/main/notebooks).

### Install JupyterLab (optional)

If you're planning to run the example notebooks and don't already have JupyterLab on your laptop, see [these instructions](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html).
