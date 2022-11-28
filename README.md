# abide_preproc_smri_freesurfer6
Data from our own pre-processing of the ABIDE I sMRI dataset (1035 subjects) in FreeSurfer v6.

Make sure to read and understand the license before using the data in this repository.

## About

This is pre-processed structural magnetic resonance imaging (sMRI) data from the [ABIDE I dataset](https://fcon_1000.projects.nitrc.org/indi/abide/abide_I.html). In short, we downloaded all 1035 ABIDE I subjects and ran their brain scans through [FreeSurfer v6](https://freesurfer.net/) `recon-all` and related tools (aseg stats, aparc start, lGI computation). The full size of the dataset is 790 GB, so we make it available in chunks.

## Abvailable data

The following data is available:

### Aggregated stats

* aggregated aparc stats (based on cortical parcellations):
   - for the Desikan atlas: thickness, area, volume
   - see see [stats directory](./stats/)
* aggregated aseg stats (based on volume segmentation):
   - aseg stats, see [stats directory ](./stats/)

### Local Gyrification Index (lGI)

 See the [native space lgi data for all ABIDE I subjects](https://doi.org/10.5281/zenodo.7132610) on Zenodo (6.5 GB download).

It includes the following files for each subject:

* `<subject>/surf/lh.pial`
* `<subject>/surf/rh.pial`
* `<subject>/surf/lh.pial_lgi`
* `<subject>/surf/rh.pial_lgi`

### Native Space Standard Surface Descriptors

See the [surface descriptor data for all ABIDE I subjects](https://zenodo.org/record/7373434) on Zenodo (6.1 GB download).

It includes the following files for each subject:

* `<subject>/surf/lh.thickness`
* `<subject>/surf/rh.thickness`
* `<subject>/surf/lh.area`
* `<subject>/surf/rh.area`
* `<subject>/surf/lh.volume`
* `<subject>/surf/rh.volume`
* `<subject>/surf/lh.curv`
* `<subject>/surf/rh.curv`
* `<subject>/surf/lh.sulc`
* `<subject>/surf/rh.sulc`
* `<subject>/surf/lh.jacobian_white`
* `<subject>/surf/rh.jacobian_white`

## License

This package contains aggregated data derived from the ABIDE I data set. That data is published under a Creative Commons, Attribution-NonCommercial-Share Alike License as explained in the [ABIDE I Usage Agreement](https://fcon_1000.projects.nitrc.org/indi/abide/abide_I.html).

Please cite the relevant ABIDE I papers when using the data for scientific publications, especially the [ABIDE I Announcing Manuscript](http://www.ncbi.nlm.nih.gov/pubmed/23774715) by Di Martino *et al*.

