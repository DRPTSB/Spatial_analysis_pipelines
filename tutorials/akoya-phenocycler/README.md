# Akoya Phenocycler (APC) Tutorials

## Overview

This section contains tutorials for analyzing data from **Akoya Biosciences Phenocycler (APC)** (formerly CODEX) platform, which provides highly multiplexed immunofluorescence imaging.

## What is Phenocycler?

Phenocycler is a spatial proteomics platform that enables:
- Highly multiplexed protein detection (40+ markers)
- Single-cell resolution imaging
- Data comes in the form of a qptiff image format which is supported by some software (e.g. qupath) but we will convert to the more brade use and standard ome.tiff format for downstream applications
## Processing pipeline for analysis with a paired Xenium sample

#### 01 - converting qptiff to ome.tiff 
- [Converting qptiff to ome.tiff with bfconvert command line](qptiff_to_ome_with_bftools.md)
  I found this option to be ideal as it produced the most robust conversion (effectively both qupath and NGFF probably use bioformats in the backhand anyway) 
- [Converting qptiff to ome.tiff with NGFF converter](qptiff_to_ome_with_NGFF.md)
- [Converting qptiff to ome.tiff with QuPath](qptiff_to_ome_with_qupath.md) 

#### 02 - image alignement between Xenium and APC
- [advanced alignent between dapi and h&e with fiji](https://www.10xgenomics.com/analysis-guides/he-to-xenium-dapi-image-registration-with-fiji)
- [image alignemnt with Xenium explorer](https://www.10xgenomics.com/support/software/xenium-explorer/latest/tutorials/xe-image-alignment)

#### 03 - Cell Segmentation
- [runnig stardist on the APC data](nuclear-segmentation.md) *(coming soon)*
- [harnassing xenium segmentation masks for APC data](cell-boundary.md) *(coming soon)*


#### 04 - Analysis Workflows




## Common Pitfalls


## Recommended Tools



## Resources

- [Akoya Biosciences Support](https://www.akoyabio.com/support/)
- [CODEX Antibody Conjugation Guide](https://www.akoyabio.com/resources/)
- [Phenocycler Panel Design Guide](https://www.akoyabio.com/phenocycler/panel-design/)

---

*Have questions? Join the [Discussion Forum](../../discussions) to connect with the community!*
