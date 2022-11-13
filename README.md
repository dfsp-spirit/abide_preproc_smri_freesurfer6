# abide_preproc_smri_freesurfer6
Data from our own pre-processing of the ABIDE I sMRI dataset (1035 subjects) in FreeSurfer v6.


## About

This is pre-processed structural magnetic resonance imaging (sMRI) data from the ABIDE I dataset. In short, we downloaded all 1035 ABIDE I subjects and ran them through FreeSurfer v6 `recon-all` and related tools (aseg stats, aparc start, lGI computation). The full size of the dataset is 790 GB, so we make it available in chunks.

## Abvailable data

The following data is available:


* aggregated aparc stats (based on cortical parcellations):
   - for the Desikan atlas: thickness, area, volume
   - see see [stats directory](./stats/)
* aggregated aseg stats (based on volume segmentation):
   - aseg stats, see [stats directory ](./stats/)

## License

* This package contains aggregated data derived from the ABIDE I data set. That data is published under a Creative Commons, Attribution-NonCommercial-Share Alike License as explained in the [ABIDE I Usage Agreement](https://fcon_1000.projects.nitrc.org/indi/abide/abide_I.html).
