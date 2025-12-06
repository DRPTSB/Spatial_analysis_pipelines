# Akoya Phenocycler (APC) Tutorials

This folder contains step-by-step tutorials for analyzing data from the Akoya Biosciences Phenocycler (formerly CODEX). Phenocycler is a high-plex immunofluorescence imaging platform that produces qptiff images; these guides show how to convert, process, segment, and analyze APC data (including workflows when pairing with Xenium samples).

Table of contents
- [Overview](#overview)
- [Processing pipeline (paired Xenium sample)](#processing-pipeline-for-analysis-with-a-paired-xenium-sample)
  - [01 — Convert qptiff → OME-TIFF](#01---convert-qptiff---ome-tiff)
  - [02 — Image alignment (Xenium ↔ APC)](#02---image-alignment-xenium--apc)
  - [03 — Cell segmentation](#03---cell-segmentation)
  - [04 — Analysis workflows](#04---analysis-workflows)
- [Common pitfalls](#common-pitfalls)
- [Recommended tools](#recommended-tools)
- [Resources](#resources)
- [Discussion](#discussion)

Overview
Phenocycler highlights
- Highly multiplexed protein detection (40+ markers)
- Single-cell resolution imaging
- Output: qptiff (we convert to OME‑TIFF for downstream tools and interoperability)

Processing pipeline for analysis with a paired Xenium sample
If you are analyzing APC data together with a Xenium sample, the typical pipeline is:
1. Convert qptiff to OME‑TIFF
2. Align images between Xenium and APC
3. Perform cell segmentation
4. Run phenotyping and spatial analyses

01 - Convert qptiff → OME‑TIFF
- Converting with Bio-Formats command line (bfconvert) — recommended for robust results  
  - tutorial: qptiff_to_ome_with_bftools.md
  - Notes: bfconvert gives consistent metadata handling across downstream tools.
- Converting with NGFF converter  
  - tutorial: qptiff_to_ome_with_NGFF.md
- Converting with QuPath  
  - tutorial: qptiff_to_ome_with_qupath.md

02 - Image alignment (Xenium ↔ APC)
- Goal: register Xenium images to APC OME‑TIFFs so coordinates/ROIs are consistent.
- Tutorial: (add link when available)
- Tips: use multi-scale rigid/affine registration first, then refine with local deformable transforms if needed.

03 - Cell segmentation
- Running StarDist on APC data (nuclei segmentation) — tutorial coming soon: nuclear-segmentation.md
- Harnessing Xenium segmentation masks for APC (use Xenium masks as priors or for QC) — tutorial coming soon: cell-boundary.md
- Comparing segmentation methods (StarDist, CellProfiler, watershed, deep-learning masks) — tutorial coming soon: segmentation-comparison.md

04 - Analysis workflows
- Cell phenotyping (marker thresholds, clustering, supervised/unsupervised labeling) — cell-phenotyping.md (coming soon)
- Spatial organization analysis (Ripley’s K, distance to structures, spatial autocorrelation) — spatial-organization.md (coming soon)
- Neighborhood enrichment (cell-type co-occurrence, permutation tests) — neighborhood-enrichment.md (coming soon)

Common pitfalls
1. Autofluorescence — include unstained controls and apply correction methods where possible.
2. Antibody cross-reactivity — validate each antibody and use appropriate controls.
3. Segmentation errors — combine nuclear and membrane markers and visually QC segmentations.
4. Batch effects — standardize staining, imaging settings, and include batch-correction in analysis.

Recommended tools
- MAV (Multiplex Analysis Viewer) — Akoya’s analysis tool
- QuPath — open-source bioimage analysis: https://qupath.github.io
- HALO — commercial digital pathology platform
- Squidpy — Python package for spatial omics: https://squidpy.org
- CellProfiler — open-source cell image analysis: https://cellprofiler.org

Resources
- Akoya Biosciences Support: https://www.akoyabio.com/support/
- CODEX / Phenocycler resources and panel design: https://www.akoyabio.com/phenocycler/
- Bio-Formats (bfconvert): https://www.openmicroscopy.org/bio-formats/

Discussion
Have questions? Join the repository Discussion Forum to connect with the community: ../../discussions

License / contribution notes
- If you update these tutorials, please follow the repository’s contribution guidelines and add small, focused changes (one topic per PR).
