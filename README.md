# pytorch-zarr-loader

## Dataset

original data used for testing:

[Link](https://imagesc.zulipchat.com/user_uploads/16804/85qPFC9O85gLhNmF5KLdqtUx/bsd_val.zarr.zip)

[Notebook for random data](create_random_test_zarr.ipynb)

## Installation

create env
```bash
mamba create -n pytorch-zarr-loader -c pytorch -c conda-forge python=3.11 ome-zarr pytorch cpuonly notebook napari matplotlib
mamba activate pytorch-zarr-loader
```

create test data
```bash
python create_random_test_zarr.py
```
