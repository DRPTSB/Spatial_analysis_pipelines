# Xenium Spatial Analysis Tutorials

## Overview

This section contains tutorials for analyzing data from **10x Genomics Xenium** platform, which provides in situ spatial transcriptomics at single-cell resolution.

## What is Xenium?

Xenium is a high-plex in situ spatial platform that enables:
- Single-cell resolution spatial transcriptomics
- Detection of hundreds of genes per cell
- Preservation of tissue architecture
- Compatibility with FFPE tissues

## Tutorials

### Getting Started
- [Introduction to Xenium Data](getting-started.md) *(coming soon)*
- [Data Loading and Preprocessing](data-loading.md) *(coming soon)*

### Quality Control
- [QC Metrics and Thresholds](qc-metrics.md) *(coming soon)*
- [Cell Segmentation Quality](cell-segmentation.md) *(coming soon)*

### Analysis Workflows
- [Cell Type Identification](cell-typing.md) *(coming soon)*
- [Spatial Gene Expression](spatial-expression.md) *(coming soon)*
- [Neighborhood Analysis](neighborhood-analysis.md) *(coming soon)*

### Advanced Topics
- [Integration with scRNA-seq](scrna-integration.md) *(coming soon)*
- [Multi-sample Analysis](multi-sample.md) *(coming soon)*

## Common Pitfalls

1. **Cell segmentation artifacts**: Over/under-segmentation can affect downstream analysis
2. **Transcript misassignment**: Consider using probabilistic methods for assignment
3. **Batch effects**: Process samples consistently and consider batch correction

## Recommended Tools

- **Xenium Analyzer**: Official 10x analysis software
- **Seurat**: R package for spatial analysis
- **Squidpy**: Python package for spatial omics
- **Giotto**: R toolkit for spatial transcriptomics

## Resources

- [10x Genomics Xenium Documentation](https://www.10xgenomics.com/support/software/xenium-analyzer)
- [Xenium Gene Panel Design Guide](https://www.10xgenomics.com/support/in-situ-gene-expression/documentation)

---

*Have questions? Join the [Discussion Forum](../../discussions) to connect with the community!*
