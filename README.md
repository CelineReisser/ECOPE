# ECOPE: Analysis of metabarcoding data
Labex-CORAIL: Impact des techniques d'élevage des huîtres perlières sur le sex ratio, la diversité génétique, et la provenance des naissains collectés.


#
## Prerequisite:
The data files we are using were already demultiplexed by the sequencing facility.

### Names of files to be analysed:
Create a "base.txt" file in the "00_scripts" folder that contain the names of individual files you want to analyse (if you have 16S and 18S data, you can for example create a base_16S.txt and a base_18S.txt). The names can be those obtained through your sequencing plateform.

### Get qza formatted databases of the silva databases:
Download the silva databases (version 132) formatted for QIIME2 (https://www.arb-silva.de/download/archive/qiime) and place it in "01_info_files". This can take a while since the file is ~3Gb.

### Get metadata
Create a sample_metadata.txt file in "01_info_files" that gather all the sampling design and attributes of your samples (e.g. origin, time of sampling...).

### Raw sequences files:
Place the raw fastq files (or their symbolic link) into the "02_data/raw/" folder


#
## Pipeline usage:

### 1. Clean the raw reads:
