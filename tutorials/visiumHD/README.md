# VisiumHD Spatial Analysis Tutorials

## Overview

This section contains tutorials for analyzing data from **10x Genomics Visium HD** platform, which provides high-definition spatial gene expression profiling.

## What is VisiumHD?

VisiumHD is a spatial transcriptomics platform that offers:
- High-resolution spatial gene expression (2µm bins)
- Whole transcriptome coverage
- Continuous tissue coverage
- Compatible with H&E and immunofluorescence imaging

## Tutorials

### Getting Started


### Quality Control
- [QC Metrics Overview](qc-metrics.md) *(coming soon)*
- [Tissue Detection QC](tissue-detection.md) *(coming soon)*
- [Spot Quality Assessment](spot-quality.md) *(coming soon)*

### Analysis Workflows
- [segmentation with bin2cell](https://github.com/Teichlab/bin2cell)


### Advanced Topics
- [Cell Type Deconvolution](deconvolution.md) *(coming soon)*
- [Integration with Single-cell Data](single-cell-integration.md) *(coming soon)*
- [Multi-resolution Analysis](multi-resolution.md) *(coming soon)*

## Common Pitfalls

1. **Bin size selection**: Choose based on tissue type and biological question
2. **Edge effects**: Be cautious when interpreting signals at tissue boundaries
3. **Library complexity**: Ensure adequate sequencing depth across the tissue

## Recommended Tools

- **Space Ranger**: 10x Genomics analysis pipeline
- **Seurat v5**: R package with native Visium HD support
- **Scanpy**: Python ecosystem for spatial analysis
- **STUtility**: R package for spatial transcriptomics

## Resources

- [10x Genomics VisiumHD Documentation](https://www.10xgenomics.com/support/software/space-ranger)
- [Visium HD Analysis Best Practices](https://www.10xgenomics.com/support/spatial-gene-expression)

---

*Have questions? Join the [Discussion Forum](../../discussions) to connect with the community!*
