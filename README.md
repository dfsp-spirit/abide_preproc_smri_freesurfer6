# abide_preproc_smri_freesurfer6
Data from our own pre-processing of the ABIDE I sMRI dataset (1035 subjects) in FreeSurfer v6.


## About

This is pre-processed structural magnetic resonance imaging (sMRI) data from the ABIDE I dataset. In short, we downloaded all 1035 ABIDE I subjects and ran them through FreeSurfer v6 `recon-all` and related tools (aseg stats, aparc start, lGI computation). The full size of the dataset is 790 GB, so we make it available in chunks.

## Abvailable data

The following data is available:

### Aggregated stats

* aggregated aparc stats (based on cortical parcellations):
   - for the Desikan atlas: thickness, area, volume
   - see see [stats directory](./stats/)
* aggregated aseg stats (based on volume segmentation):
   - aseg stats, see [stats directory ](./stats/)

### native space local Gyrification Index (lGI)

 See the [native space lgi data for all ABIDE I subjects](https://doi.org/10.5281/zenodo.7132610) on Zenodo (6.5 GB download).

The download includes only the files required for meshlearn training, for the ABIDE I dataset. These are the following files per subject:

* `<subject>/surf/lh.pial`
* `<subject>/surf/rh.pial`
* `<subject>/surf/lh.pial_lgi`
* `<subject>/surf/rh.pial_lgi`

## License

* This package contains aggregated data derived from the ABIDE I data set. That data is published under a Creative Commons, Attribution-NonCommercial-Share Alike License as explained in the [ABIDE I Usage Agreement](https://fcon_1000.projects.nitrc.org/indi/abide/abide_I.html).
