## SeATAC: A tool for exploring the chromatin landscape and the role of pioneer factors

Nikita Dsouza, Wuming Gong and Daniel J. Garry


## Main Figures


### Figure 1

|  | Figures | Link | 
| --- | --- | --- | 
|  A full V-plot has a width of 640 bp genomic region and a height of 640 bp of fragment sizes. An array of 5 x 10 pixels are aggregated together and become a single larger pixel, resulting in a 128 x 64 pixels image. | Figure 1a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Vplot_demo_1a.ipynb) |
| SeATAC models the ATAC-seq V-plot using a conditional variational autoencoder (CVAE) framework. | Figure 1b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Vplot_demo_1a.ipynb) |
| Four separate tasks for evaluating the performance of detecting chromatin accessibility changes. | Figure 1c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Vplot_demo_1a.ipynb) |


### Figure 2
|  | Figures | Link | 
| --- | --- | --- | 
|  SeATAC detects differential V-plots. | Figure 2a | |
| Different tools are used to compare dataset #1 vs. dataset #2, and dataset #1 vs. dataset #3 to detect differential V-plots. | Figure 2b | |
| The ROC curves for SeATAC, NucleoATAC and MACS2 for four different shift sizes: 10, 20, 50 and 100 bp are shown | Figure 2c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/GM12878_SeATAC_MACS2_compare_v2.ipynb) |


### Figure 3
|  | Figures | Link | 
| --- | --- | --- | 
|  The ROC curve for recovering nucleosome positions from ATAC-seq with 0.1%, 1% and 10% of the sequencing reads randomly sampled from the full dataset (GM12878). | Figure 3a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/GM12878_nucleosome_calling_f3%20.ipynb) |
| The heatmaps shows the nucleosome density estimated by SeATAC (blue) and NucleoATAC (purple) on a 1% down-sampled dataset. | Figure 3b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/GM12878_nucleosome_calling_f3%20.ipynb) |

### Figure 4
|  | Figures | Link | 
| --- | --- | --- | 
| The ROC curve for detecting nucleosome changes from ATAC-seq with 10% of the sequencing reads from the full dataset (GM12878). | Figure 4a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/GM12878_diff_nuc_f4ac.ipynb) |
| The raw and estimated V-plot of a NFR (chr1:113162059-113162698) and a NOR (chr2:226653061-226653700) region are shown | Figure 4b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/GM12878_diff_nuc_f4ac.ipynb) |
| The heatmaps show the nucleosome density of ~5,000 sampled NOR and NFR regions estimated by SeATAC & NucleoATAC  on a 10% down-sampled dataset and NucleoATAC signal on the full dataset (black) & a MNase-seq dataset on GM12878. |  Figure 4c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/GM12878_diff_nuc_f4ac.ipynb) |

### Figure 5
|  | Figures | Link | 
| --- | --- | --- | 
| The Venn diagrams show the number of Etv2 motifs with increased chromatin accessibility identified by SeATAC, MACS2 and NucleoATAC Etv2 induced MEF. | Figure 5a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Etv2_MEF_and_EB_v0_4_0_pathway_analysis_f5.ipynb) |
| The Venn diagrams show the number of Etv2 motifs with increased chromatin accessibility identified by SeATAC, MACS2 and NucleoATAC Etv2 induced EB differentiation | Figure 5b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Etv2_MEF_and_EB_v0_4_0_pathway_analysis_f5.ipynb) |
| The aggregated V-plot includes 1,626, 222 and 2,305 Etv2 motifs with increased chromatin accessibility identified by SeATAC only, MACS2 only and NucleoATAC only in ATAC-seq data of Etv2 induced EB differentiation | Figure 5c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Etv2_EB_v0_4_0_Vplots_for_and_EBs_Figure.ipynb) |
|  The barplots show the Gene Ontology (GO) terms that are significantly associated with the genes which promoters (-5,000 - +1,000bp region flanking the TSS) have Etv2 motifs with increased chromatin accessibility, identified by SeATAC, MACS2 and NucleoATAC. | Figure 5d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Etv2_MEF_and_EB_v0_4_0_pathway_analysis_f5.ipynb) |

### Figure 6
|  | Figures | Link | 
| --- | --- | --- | 
| Dot plots comparing the changes of motif associated chromatin accessibility estimated by chromVAR (x-axis) and the difference of the percent of TFBS with decreased or increased chromatin accessibility estimated by SeATAC. | Figure 6a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Etv2_MEF_EB_motifs.ipynb) |
| The barplots show the genomic distribution of Etv2 binding sites with decreased (NFR->NOR) or increased (NOR->NFR) chromatin accessibility in EB differentiation or MEF reprogramming. | Figure 6b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Etv2_MEF_EB_Etv2_v1.ipynb) |
| The aggregated V-plot include 3,000 and 1,623 Etv2 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during MEF reprograming. | Figure 6c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Etv2_MEF_EB_Etv2_v1.ipynb) |
| The heatmaps showing Etv2, Brg1, H3K27ac ChIP-seq of 3,000 and 1,623 Etv2 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility at day 2.5 EB (Brg1 and H3K27ac), 3 hours post Etv2 induction (Etv2), and 12 hours post Etv2 induction (Etv2, Brg1 and H3K27ac). | Figure 6d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Etv2_MEF_EB_Etv2_v1.ipynb) |
| The barplots show the percent of genes that were down-regulated, up-regulated or not changed between day 2.5 EB and 12 hours post Etv2 induction. | Figure 6e | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/EB_RNA_and_NOR_NFR_f6ef.ipynb) |
| Brachyury (T) and Mycn are significantly down-regulated during the Etv2 induced differentiation. | Fgure 6f | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/EB_RNA_and_NOR_NFR_f6ef.ipynb) |
| Brachyury (T) and Mycn (f) have Etv2 motifs that become significantly less accessible during the differentiation at their promoter region (-5,000 - +1,000bp region flanking the TSS) | Figure 6g | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Vplots_for_and_EBs_specific_genes.ipynb) |

## Supplementary Figure


### Supplementary Figure 1
|  | Figures | Link | 
| --- | --- | --- |
| The density plots show the observed (red) and corrected (green) fragment size distribution of 13 samples from a human hematopoietic differentiation ATAC-seq data (GSE96771). | Supplementary Figure 1a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_corrects_batch_effects_sf1.ipynb) |

### Supplementary Figure 2
|  | Figures | Link | 
| --- | --- | --- |
| The aggregated V-plot includes 2,776, 116 and 1,449 Etv2 motifs with increased chromatin accessibility identified by SeATAC only, MACS2 only and NucleoATAC only in ATAC-seq data of Etv2 induced MEF reprogramming | Supplementary Figure 2a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Etv2_MEF_v0_4_0_Vplots_for_and_MEFs_Figure.ipynb) |
| The heatmaps show the Etv2, Brg1, H3K27ac ChIP-seq of 3,996 and 1,307 Etv2 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility at undifferentiated MEFs (Brg1 and H3K27ac), 1 day post-Etv2 induction (Etv2), and 7 days post-Etv2 induction (Etv2, Brg1 and H3K27ac). | Supplementary Figure 2b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Etv2_MEF_EB_Etv2_v1.ipynb)| 
| The UCSC genome browser track show the ATAC-seq density near the Etv2 motifs at the promoters of Brachyury (T) and Mycn. | Supplementary Figure 2c | [T](https://genome.ucsc.edu/s/ndsouza/T_new) <br> [Mycn](https://genome.ucsc.edu/s/ndsouza/Mycn_new) |

### Supplementary Figure 3
|  | Figures | Link | 
| --- | --- | --- |
| The Venn diagrams show the number of Ascl1 motifs with increased chromatin accessibility identified by SeATAC, MACS2 and NucleoATAC. | Supplementary Figure 3a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Ascl1_MEFs_D22_analysis_sf3.ipynb) |
| The barplots show the Gene Ontology (GO) terms that are significantly associated with the genes which promoters (-5,000 - +1,000bp region flanking the TSS) have Ascl1 motifs with increased chromatin accessibility, identified by SeATAC, MACS2 and NucleoATAC.  | Supplementary Figure 3b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Ascl1_MEFs_D22_analysis_sf3.ipynb) |
| The aggregated V-plot includes 8,658, 7,687 and 7,708 Ascl1 motifs with increased chromatin accessibility identified by SeATAC only, MACS2 only and NucleoATAC only in ATAC-seq data of Ascl1 induced MEF reprogramming (undifferentiated MEFs vs. 22 days post Ascl1 induction). | Supplementary Figure 3c |  [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Ascl1_MEFs_D22_analysis_sf3.ipynb) |

### Supplementary Figure 4
|  | Figures | Link | 
| --- | --- | --- |
| The Venn diagrams show the number of OSK motifs with increased chromatin accessibility identified by SeATAC, MACS2 and NucleoATAC. | Supplementary Figure 4a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_OSK_MEFs_D7_sf4.ipynb) |
| The barplots show the Gene Ontology (GO) terms that are significantly associated with the genes which promoters (-5,000 - +1,000bp region flanking the TSS) have OSK motifs with increased chromatin accessibility, identified by SeATAC, MACS2 and NucleoATAC. | Supplementary Figure 4b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_OSK_MEFs_D7_sf4.ipynb) |
| The aggregated V-plot includes 5,826, 1,355 and 6,371 OSK motifs with increased chromatin accessibility identified by SeATAC only, MACS2 only and NucleoATAC only in ATAC-seq data of OSK induced MEF reprogramming | Supplementary Figure 4c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_OSK_MEFs_D7_sf4.ipynb) |

### Supplementary Figure 5
|  | Figures | Link | 
| --- | --- | --- |
| The dot plots compare the changes of motif associated chromatin accessibility estimated by chromVAR (x-axis) and the difference of the percent of TFBS with decreased or increased chromatin accessibility estimated by SeATAC | Supplementary Figure 5a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Ascl1_MEF_motifs.ipynb) |
| The barplots show the genomic distribution of Ascl1 binding sites with decreased (NFR->NOR) or increased (NOR->NFR) chromatin accessibility in MEF reprogramming. | Supplementary Figure 5b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Ascl1_MEF_Seatac_Supplementary_v1.ipynb) |
| The aggregated V-plot include 24,098 and 7,071 Ascl1 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during MEF reprograming. | Supplementary Figure 5c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Ascl1_MEF_Seatac_Supplementary_v1.ipynb) |
| The heatmaps show the MNase-seq, H3K27m3, H3K36m3, H3K9ac, H3K79me2, H3K4me2, H3K4me1 and P300 ChIP-seq signals in undifferentiated MEFs of 24,098 and 7,071 Ascl1 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during the MEF reprogramming. | Supplementary Figure 5d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Ascl1_MEF_Seatac_Supplementary_v1.ipynb) |
| The V-plot show Ascl1 motifs with decreased chromatin accessibility at the promoters (-5,000 - +1,000bp region flanking the TSS) of four genes (Hmga2, Elf4, Egfr and Hes1) that are down-regulated during the Ascl1 induced MEF reprogramming. | Supplementary Figure 5e | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Ascl1_MEFs_D22_specific_genes_sf5e.ipynb) |

### Supplementary Figure 6
|  | Figures | Link | 
| --- | --- | --- |
| The dot plots compare the changes of motif associated chromatin accessibility estimated by chromVAR (x-axis) and the difference of the percent of TFBS with decreased or increased chromatin accessibility estimated by SeATAC | Supplementary Figure 6a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/OSK_MEF_motifs.ipynb) |
| The barplots show the genomic distribution of OSK binding sites with decreased (NFR->NOR) or increased (NOR->NFR) chromatin accessibility in MEF reprogramming. | Supplementary Figure 6b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/OSK_MEF_Seatac_Supplementary.ipynb) |
| The aggregated V-plot include 15,825 and 4,935 OSK binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during MEF reprograming. | Supplementary Figure 6c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/OSK_MEF_Seatac_Supplementary.ipynb) |
| The heatmaps show the MNase-seq, H3K27m3, H3K36m3, H3K9ac, H3K79me2, H3K4me2, H3K4me1 and P300 ChIP-seq signals in undifferentiated MEFs of 15,825 and 4,935 OSK binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during the MEF reprogramming. | Supplementary Figure 6d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/OSK_MEF_Seatac_Supplementary.ipynb) |
| The barplots show the percent of genes that were down-regulated, up-regulated or not changed between undifferentiated MEFs and 7 hours post OSK induction. | Supplementary Figure 6e | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/OSK_RNA_and_NOR_NFR_sf6ef.ipynb) |
| Maf and Smad3 are significantly down-regulated during the OSK induced MEF reprogramming. | Supplementary Figure 6f | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/OSK_RNA_and_NOR_NFR_sf6ef.ipynb)  |
| Maf and Smad3 have OSK motifs that become significantly less accessible during the differentiation at their promoter region (-5,000 - +1,000bp region flanking the TSS). | Supplementary Figure 6g | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_OSK_MEFs_D7_specific_genes_sf6g.ipynb) |
