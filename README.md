# abide_preproc_smri_freesurfer6
Data from our own pre-processing of the ABIDE I sMRI dataset (1035 subjects) in FreeSurfer v6.

Make sure to read and understand the license before using the data in this repository.

## About

This is pre-processed structural magnetic resonance imaging (sMRI) data from the [ABIDE I dataset](https://fcon_1000.projects.nitrc.org/indi/abide/abide_I.html). In short, we downloaded all 1035 ABIDE I subjects and ran their brain scans through [FreeSurfer v6](https://freesurfer.net/) `recon-all` and related tools (aseg stats, aparc start, lGI computation). The full size of the dataset is 790 GB, so we make it available in chunks.

The uploaded archives are very large already (> 30 GB), so we opted not to upload log files and other parts of the FreeSurfer 6 output which are typically not relevant for neuroimaging research. We have the full data though, and if you feel you require a file that is missing, we can add that file for all subjects in another upload. Please get in touch by [opening an issue](https://github.com/dfsp-spirit/abide_preproc_smri_freesurfer6/issues) in that case.

## Available data

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

### Brain Surfaces (Meshes)

See the [brain surfaces for all ABIDE I subjects](https://zenodo.org/record/7373936) on Zenodo (16.3 GB download).

It includes the following files for each subject:

* `<subject>/surf/lh.white`
* `<subject>/surf/rh.white`
* `<subject>/surf/lh.orig`
* `<subject>/surf/rh.orig`
* `<subject>/surf/lh.sphere`
* `<subject>/surf/rh.sphere`

Note: The pial surface files are part of the `Local Gyrification Index` dataset, see above.

### Labels

See the [labels for all ABIDE I subjects](https://zenodo.org/record/7377435) on Zenodo (4.7 GB download).

It includes the following files for each subject:

* `<subject>/label/lh.cortex.label`
* `<subject>/label/rh.cortex.label`
* `<subject>/label/lh.aparc.annot`
* `<subject>/label/rh.aparc.annot`
* `<subject>/label/lh.aparc.a2009s.annot`
* `<subject>/label/rh.aparc.a2009s.annot`

### Volumes (the 3D MRI images)

See the [Brain volumnes for all ABIDE I subjects](https://doi.org/10.5281/zenodo.8068739) on Zenodo (3.1 GB download).

It includes the following files for each subject:

* `<subject>/mri/brain.mgz`
* `<subject>/mri/brain_mask.mgz`
* `<subject>/mri/aseg.mgz`
* `<subject>/mri/wm.mgz`

## License

This package contains aggregated data derived from the ABIDE I data set. That data is published under a Creative Commons, Attribution-NonCommercial-Share Alike License as explained in the [ABIDE I Usage Agreement](https://fcon_1000.projects.nitrc.org/indi/abide/abide_I.html).

Please cite the relevant ABIDE I papers when using the data for scientific publications, especially the [ABIDE I Announcing Manuscript](http://www.ncbi.nlm.nih.gov/pubmed/23774715) by Di Martino *et al*.

