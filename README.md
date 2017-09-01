Readme for ./run_otus.sh  

This script will process paired end data through the vsearch pipeline.  

Modified from https://github.com/torognes/vsearch/wiki/VSEARCH-pipeline  

### Requirements  
- Fastq R1 and R2 files ending in either .fastq or fastq.gz.  
- Filenames contain the sample name in full without special characters  
- Fastq files are copied to ./projectData  

The sample name is extracted by `cut -d_ -f1`:  
The following filenames are acceptable:  
MHApr13_S30_L001_R1_001.fastq.gz   
MHApr13_S30_L001_R2_001.fastq.gz   
MHApr14_S30_L001_R2_001.fastq.gz  
MHApr14_S30_L001_R2_001.fastq.gz  
MHApr15_S30_L001_R2_001.fastq.gz  
MHApr15_S30_L001_R2_001.fastq.gz  

These are NOT compatible because MHApr13 is not uq, use MHApr13S30 as
 sample name by removing _.  
MHApr13_S30_L001_R1_001.fastq.gz   
MHApr13_S30_L001_R1_001.fastq.gz   
MHApr13_S31_L001_R2_001.fastq.gz   
MHApr13_S31_L001_R2_001.fastq.gz   

### Key Paramaters  

V2 V3-V4 V4  

### Key outputs  
The uc format is described here:
http://www.drive5.com/usearch/manual/opt_uc.html  

