# Akoya Phenocycler Tutorials

## Overview

This section contains tutorials for analyzing data from **Akoya Biosciences Phenocycler** (formerly CODEX) platform, which provides highly multiplexed immunofluorescence imaging.

## What is Phenocycler?

Phenocycler is a spatial proteomics platform that enables:
- Highly multiplexed protein detection (40+ markers)
- Single-cell resolution imaging
- Subcellular localization analysis
- Compatible with FFPE and fresh frozen tissues

## Tutorials

### Getting Started
- [Introduction to Phenocycler Data](getting-started.md) *(coming soon)*
- [Understanding the CODEX Workflow](codex-workflow.md) *(coming soon)*

### Initial Processing
- [Converting qptiff to ome.tiff](qptiff_to_ome.md) *(coming soon)*
- [tbd](crosstalk-correction.md) *(coming soon)*

### Cell Segmentation
- [Nuclear Segmentation](nuclear-segmentation.md) *(coming soon)*
- [Cell Boundary Detection](cell-boundary.md) *(coming soon)*
- [Comparing Segmentation Methods](segmentation-comparison.md) *(coming soon)*

### Analysis Workflows
- [Marker Intensity Normalization](normalization.md) *(coming soon)*
- [Cell Phenotyping](cell-phenotyping.md) *(coming soon)*
- [Spatial Organization Analysis](spatial-organization.md) *(coming soon)*
- [Neighborhood Enrichment](neighborhood-enrichment.md) *(coming soon)*

### Advanced Topics
- [Multi-tissue Analysis](multi-tissue.md) *(coming soon)*
- [Panel Optimization](panel-optimization.md) *(coming soon)*
- [Machine Learning for Phenotyping](ml-phenotyping.md) *(coming soon)*

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
