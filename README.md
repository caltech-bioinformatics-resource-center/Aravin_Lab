# Aravin_Lab
#### This github repository includes piRNA RNAseq data processing pipelines for a research article [XYZ](https://).  
#### The codes can be used under UNIX(Centos/Ubuntu) environment with proper installation of necessary software tools.
####
#### Directory contents 
* [run_alignment] A bash script to align piRNA RNAseq data and collect multi-mapped and uniquely-mapped reads.
* [run_multi_reads_for_rev] A bash script for creating a normalized multi-mapped and uniquely-mapped signal trace files (bedgraph) for visualization. 
* [run_dist] A bash script to calculate intra-chromosomal span of multi-mapped reads.

#### Quick run:
* Install piRNA RNAseq processing codes `git clone https://github.com/caltech-bioinformatics-resource-center/Aravin_Labs.git`. 
* Relocate to local piRNA code directory `cd Aravin_Lab`.
* Transfer raw single-end fastq.gz files to the piRNA code directory.
* Modify `sample_ID.txt` file to include data IDs of raw single-end fastq files. Also include local PATH information for bowtie2, bowtie2 index, samtools, deeptools, bedtools, macs2 in `run_alignment` and `run_multi_reads_for_rev` files.
* Run alignment `bash run_alignment`.
* Run further analysis for uniquely and multi-mapped reads `bash run_multi_reads_for_rev`.
####
