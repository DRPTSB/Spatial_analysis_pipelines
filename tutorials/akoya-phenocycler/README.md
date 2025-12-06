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
- [Converting qptiff to ome.tiff with NGFF converter](qptiff_to_ome_with_NGFF.md)
- [Converting qptiff to ome.tiff with QuPath](qptiff_to_ome_with_qupath.md) 

#### 02 - image alignement between Xenium and APC

#### 03 - Cell Segmentation
- [runnig stardist on the APC data](nuclear-segmentation.md) *(coming soon)*
- [harnassing xenium segmentation masks for APC data](cell-boundary.md) *(coming soon)*
- [Comparing Segmentation Methods](segmentation-comparison.md) *(coming soon)*

#### 04 - Analysis Workflows
- [Cell Phenotyping](cell-phenotyping.md) *(coming soon)*
- [Spatial Organization Analysis](spatial-organization.md) *(coming soon)*
- [Neighborhood Enrichment](neighborhood-enrichment.md) *(coming soon)*



## Common Pitfalls

1. **Autofluorescence**: Proper controls and correction are essential
2. **Antibody cross-reactivity**: Validate panels thoroughly
3. **Segmentation errors**: Use multiple nuclear and membrane markers when possible
4. **Batch effects**: Standardize staining and imaging protocols

## Recommended Tools

- **MAV (Multiplex Analysis Viewer)**: Akoya's analysis software
- **QuPath**: Open-source bioimage analysis
- **HALO**: Digital pathology platform
- **Squidpy**: Python package for spatial omics
- **CellProfiler**: Open-source cell image analysis

## Resources

- [Akoya Biosciences Support](https://www.akoyabio.com/support/)
- [CODEX Antibody Conjugation Guide](https://www.akoyabio.com/resources/)
- [Phenocycler Panel Design Guide](https://www.akoyabio.com/phenocycler/panel-design/)

---

*Have questions? Join the [Discussion Forum](../../discussions) to connect with the community!*
