This is a pipeline I modified to combine multi-modal multiome datasets across two conditions: control and knockdown of a histone variant. It uses Seurat v5.1.0 and Signac v1.14.0 to analyse, integrate and visualise differences across conditions
The kit used for the run was 10X Genomics Single cell ATAC + 3' Gene Expression kit and it was sequenced on Illumina NextSeq 1000 platform
The input files are:
1) .h5 count matrix 
2) .tsv.gz fragments file
3) .barcode_metrics.csv file, all generated by Cellranger arc-v8 pipeline

The experiment was carried out in 28-30 hpf sox10+/gfp zebrafish (Danio rerio) embryos and the pipeline was constructed using standard Seurat and Signac vignettes with minor modifications, just as ATAC normalization performed twice
This pipeline effectively merges the multiple layers of the data, and minimizes the batch effects