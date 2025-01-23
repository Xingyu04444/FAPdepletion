# FAPdepletion

Data analysis in this paper are mostly based on developed R packages. Here we provided a brief workflow while detailed codes can be found in corresponding files.

Part I Software & Dependencies 
All codes are R-based, running on RStudio (version 4.3.2). Dependencies were listed as below:

```
R version 4.3.2 (2023-10-31 ucrt)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows 11 x64 (build 26100)

attached base packages:
[1] stats4    stats     graphics  grDevices utils     datasets 
[7] methods   base     

other attached packages:
 [1] CellChat_2.1.1              igraph_2.0.3               
 [3] EnhancedVolcano_1.20.0      SeuratWrappers_0.3.0       
 [5] monocle3_1.0.0              SingleCellExperiment_1.24.0
 [7] SummarizedExperiment_1.32.0 GenomicRanges_1.54.1       
 [9] GenomeInfoDb_1.38.8         MatrixGenerics_1.14.0      
[11] matrixStats_1.3.0           org.Mm.eg.db_3.18.0        
[13] AnnotationDbi_1.64.1        IRanges_2.36.0             
[15] S4Vectors_0.40.2            Biobase_2.62.0             
[17] BiocGenerics_0.48.1         clusterProfiler_4.10.1     
[19] gprofiler2_0.2.3            nichenetr_2.0.4            
[21] harmony_1.2.0               Rcpp_1.0.12                
[23] reshape2_1.4.4              lubridate_1.9.3            
[25] forcats_1.0.0               stringr_1.5.1              
[27] purrr_1.0.2                 readr_2.1.5                
[29] tidyr_1.3.0                 tibble_3.2.1               
[31] tidyverse_2.0.0             future_1.33.2              
[33] ggrepel_0.9.5               RColorBrewer_1.1-3         
[35] ggplot2_3.5.1               cowplot_1.1.3              
[37] Matrix_1.6-5                patchwork_1.2.0            
[39] dplyr_1.1.4                 Seurat_5.0.3               
[41] SeuratObject_5.0.1          sp_2.1-2
           
```



Part II Single-cell level data analysis
i. Quality control and single-cell cluserting
Please refer to files "1_homeostasis_data_processing.Rmd" and "2_inj_data_processing.Rmd".
To investigate specific cell types at a higher resolution by subclustering, please refer to files "3_all_reclustering.Rmd" and "4_FAPTenoSC_recluster_special.Rmd".

ii. Inferring cell-cell interaction networks
Please refer to file "5_CellChat.Rmd".

iii. Predicting the regulatory potential and mechanisms of FAP-derived signals
Please refer to file "6_NicheNet.Rmd".

iv. Constructing trajectory of neutrophil subpopulations along developmental stage in homeostatic muscle
Please refer to file "7_Trajectory inference.Rmd".

v. Other functional codes
For codes generating volcano plots (showing differentially expressed genes) and conducting gene ontology analysis/pathway enrichment analysis,
 please refer to file "8_not classified scripts.Rmd".

