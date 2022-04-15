# seatac_manuscript

## SeATAC: A tool for exploring the chromatin landscape and the role of pioneer factors

## Main Figures

### Figure 1

|  | Figures | Link | 
| --- | --- | --- | 
|  A full V-plot has a width of 640 bp genomic region and a height of 640 bp of fragment sizes. An array of 5 x 10 pixels are aggregated together and become a single larger pixel, resulting in a 128 x 64 pixels image. | Figure 1a | |
| SeATAC models the ATAC-seq V-plot using a conditional variational autoencoder (CVAE) framework. | Figure 1b | |
| Four separate tasks for evaluating the performance of detecting chromatin accessibility changes. | Figure 1c | |


### Figure 2
|  | Figures | Link | 
| --- | --- | --- | 
|  SeATAC detects differential V-plots. | Figure 2a | |
| Different tools are used to compare dataset #1 vs. dataset #2, and dataset #1 vs. dataset #3 to detect differential V-plots. | Figure 2b | |
| The ROC curves for SeATAC, NucleoATAC and MACS2 for four different shift sizes: 10, 20, 50 and 100 bp are shown | Figure 2c | |


### Figure 3
|  | Figures | Link | 
| --- | --- | --- | 
|  The ROC curve for recovering nucleosome positions from ATAC-seq with 0.1%, 1% and 10% of the sequencing reads randomly sampled from the full dataset (GM12878). | Figure 3a | |
| The heatmaps shows the nucleosome density estimated by SeATAC (blue) and NucleoATAC (purple) on a 1% down-sampled dataset. | Figure 3b | |

### Figure 4
|  | Figures | Link | 
| --- | --- | --- | 
| The ROC curve for detecting nucleosome changes from ATAC-seq with 10% of the sequencing reads from the full dataset (GM12878). | Figure 4a | |
| The raw and estimated V-plot of a NFR (chr1:113162059-113162698) and a NOR (chr2:226653061-226653700) region are shown | Figure 4b | |
| The heatmaps show the nucleosome density of ~5,000 sampled NOR and NFR regions estimated by SeATAC & NucleoATAC  on a 10% down-sampled dataset and NucleoATAC signal on the full dataset (black) & a MNase-seq dataset on GM12878. |  Figure 4c | |
