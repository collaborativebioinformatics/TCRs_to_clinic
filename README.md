# TCRs_to_clinic

### Contributors:

* Ankita Das
* Sheethal Umesh Nagalakshmi

## Goals

* Monitor immunotherapy treatment (TCR clonotype over time)
* Diagnosing disease early with TCR clonality change in blood

## Introduction

## Methods 

* FASTQ files obtained from TCR a/b/g/d sequencing 
* Run this through automated pipelines available on DNAnexus and a Jupyter lab version
* Analyze Bulk TCR Takara or 5’RACE or Multiplex PCR using ClonoMap Immune Profiler and Immunearch 
* Analyze TCR data using Immunarch for data visualization

### Running the ClonoMap Immune Profiler pipeline on DNAnexus 
<img width="656" alt="Screen Shot 2021-06-04 at 11 08 00 AM" src="https://user-images.githubusercontent.com/74208394/120845076-262edf80-c525-11eb-9a2d-d270d0256cb5.png">

### Running the ClonoMap paired end pipeline with FASTQ files 
<img width="619" alt="Screen Shot 2021-06-04 at 11 06 25 AM" src="https://user-images.githubusercontent.com/74208394/120844941-f7186e00-c524-11eb-8bf8-b0b691c85e96.png">

### Upload metedata file to go with the files and run Immunarch
<img width="426" alt="Screen Shot 2021-06-04 at 11 09 20 AM" src="https://user-images.githubusercontent.com/74208394/120845246-62fad680-c525-11eb-86ce-dd835d992306.png">

## Implementation

### Input:

#### Bulk TCR Takara or 5’RACE or Multiplex PCR analysis using ClonoMap Immune Profiler and Immunearch 

Paired or single end Fastq files generated from the respective chemistries for TCR a/b/g/d sequencing 

#### TCR data analysis using Immunarch 

Path for single or list of repertoire files.

### Package installation

Automated pipelines are available on DNAnexus. 
Jupyter lab version is available to institute on any other environment.
Immunarch package can be installed following instruction s here: https://immunarch.com/

#### Running the ClonoMap Immune Profiler pipeline on DNAnexus 



### Output:

TSV of clones 
Immunearch generated Pdf reports that can be downloaded. 
TCR data visualization graphs from Immunarch can be downloaded.

### Number of clones and distributions of clones 

![Number_of_clonotypes](https://user-images.githubusercontent.com/41301333/120838746-15e82600-c560-11eb-8367-88fd636d93cc.png)

### Relative abundance of clonotypes

![relative_abundance](https://user-images.githubusercontent.com/41301333/120838748-1680bc80-c560-11eb-9f96-cbac19abe30c.png)

### Clonotype tracking

![clonotype_tracking_line](https://user-images.githubusercontent.com/41301333/120838744-14b6f900-c560-11eb-8587-a2b251035365.png)

### Diversity analysis

![sample_diversity](https://user-images.githubusercontent.com/41301333/120838751-1680bc80-c560-11eb-88ae-ecd871ad445e.png)


## References:

ImmunoMind Team. (2019). immunarch: An R Package for Painless Bioinformatics Analysis of T-Cell and B-Cell Immune Repertoires. Zenodo. http://doi.org/10.5281/zenodo.3367200

Samir, J., Rizzetto, S., Gupta, M. et al. Exploring and analysing single cell multi-omics data with VDJView. BMC Med Genomics 13, 29 (2020). https://doi.org/10.1186/s12920-020-0696-z

