# QPTIFF to OME-TIFF Processing with bftools

This guide outlines the steps to convert QPTIFF files to OME-TIFF using `bftools`, including generating specific files for Xenium Explorer alignment.

## Step 1: Installation

1. Download the **command line tools** for `bftools` from [here](https://www.openmicroscopy.org/bio-formats/downloads/).
2. Follow the installation instructions included in the download.
3. **Note:** You may need to install or update Java/JDK for these tools to function.

## Step 2: Setup

Open your terminal (or cmd) and navigate to your `bftools` directory:

```bash
cd ~/path/to/bftools
````

## Step 3: General Conversion

Run the following to generate an OME-TIFF from your QPTIFF with the necessary pyramid parameters:

```bash
./bfconvert \
  -noflat \
  -pyramid-resolutions 5 \
  -pyramid-scale 2 \
  -tilex 1024 \
  -tiley 1024 \
  -compression zlib \
  /path-to-file/scan.qptiff \
  /path-to-file/scan.qptiff.ome.tiff
```

## Step 4: Generate DAPI Channel for Xenium Alignment

We need to generate a separate OME-TIFF of **only the DAPI channel** (typically Channel 0/CH0). This is required for alignment within [Xenium Explorer](https://www.10xgenomics.com/support/software/xenium-explorer/latest/tutorials/xe-image-file-conversion).

Because handling pyramidal files directly can be difficult, we perform this in two steps:

### A) Extract the first channel (CH0)

First, generate a temporary non-pyramidal file of just the first channel.

```bash
./bfconvert \
  -series 0 \
  -channel 0 \
  -compression zlib \
  /Volumes/ThymusAtlas/shani_data/akoya/J18J19_Slide2_Scan1.er.qptiff.ome.tiff \
  /Volumes/ThymusAtlas/shani_data/akoya/temp_CH0.ome.tiff
```

### B) Convert to Pyramidal Format

Convert the temporary non-pyramidal file into the final pyramidal OME-TIFF required by Xenium.

```bash
./bfconvert \
  -pyramid-resolutions 5 \
  -pyramid-scale 2 \
  -tilex 1024 \
  -tiley 1024 \
  -compression zlib \
  /Volumes/ThymusAtlas/shani_data/akoya/temp_CH0.ome.tiff \
  /Volumes/ThymusAtlas/shani_data/akoya/J18J19_Slide2_Scan1.er.CH0_pyr.ome.tiff
```

