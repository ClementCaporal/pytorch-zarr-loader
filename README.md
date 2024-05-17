# pytorch-zarr-loader

During the Biovision Hackathon 2023 in Zurich we wanted to find a way to load data from a zarr file into pytorch. The goal was to load the data in a way that it can be used for training a neural network.
We tried several solution in particular using or without using dask to load the data in parallel.

## Dataset

original data used for testing:[Link](https://imagesc.zulipchat.com/user_uploads/16804/85qPFC9O85gLhNmF5KLdqtUx/bsd_val.zarr.zip)
But you can also find an example to generate a random data : 
- [Notebook for random data](create_random_test_zarr.ipynb)
- [Notebook for huge random data zarr and tiff](create_huge_random_zarr_and_tif)

Proposed loaders:
- [Fastest loader](example_ZARR.ipynb)
- [Notebook for dask loader](dask_future_loader_zarr.ipynb)

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
## Similar solutions

Please consider other repo that also load zarr for pytorch
- https://github.com/TheJacksonLaboratory/zarrdataset
