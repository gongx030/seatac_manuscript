## SeATAC: A tool for exploring the chromatin landscape and the role of pioneer factors

Wuming Gong, Nikita Dsouza and Daniel J. Garry

## Abstract

Assay for Transposase-Accessible Chromatin with sequencing (ATAC-seq) reveals chromatin accessibility across the genome. Currently no method specifically detects differential chromatin accessibility. Here, SeATAC uses a conditional variational autoencoder model to learn the latent representation of ATAC-seq V-plots and outperforms MACS2 and NucleoATAC on six separate tasks. Applying SeATAC to several pioneer factor induced differentiation or reprogramming ATAC-seq datasets suggests that induction of these factors not only relaxes the closed chromatin but also decreases chromatin accessibility of 20% to 30% of their target sites. SeATAC is a novel tool to accurately reveal genomic regions with differential chromatin accessibility from ATAC-seq data. SeATAC is available at https://github.com/gongx030/seatac as an R package. The preprint can be found at [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.04.25.489439v1).  

## Main Figures


### Figure 1

|  | Figures | Link | 
| --- | --- | --- | 
|  A full V-plot has a width of 640 bp genomic region and a height of 640 bp of fragment sizes. An array of 5 x 10 pixels are aggregated together and become a single larger pixel, resulting in a 128 x 64 pixels image. | Figure 1a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Vplot_demo_1a.ipynb) |

### Figure 2
|  | Figures | Link | 
| --- | --- | --- | 
| The ROC curves for SeATAC, NucleoATAC and MACS2 with a shift size of 50 bp.| Figure 2c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/seatac_GM12878_task1.ipynb) |
| The violin plot shows the AUC (area under ROC) of SeATAC, NucleoATAC and MACS2 on 523 ATAC-seq samples from 20 studies. *** Wilcoxon rank sum test p-value < 0.001. | Figure 2d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/summarize_comp.ipynb) |
| The AUC of SeATAC, NucleoATAC and MACS2 at different read counts cutoff from 1 to 20 (the minimum reads in a V-plot).| Figure 2e | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/summarize_comp.ipynb) |

### Figure 3
|  | Figures | Link | 
| --- | --- | --- | 
|  The ROC curve for recovering nucleosome positions from ATAC-seq with 0.1%, 1% and 10% of the sequencing reads randomly sampled from the full dataset (GM12878). | Figure 3a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/GM12878_nucleosome_calling_f3%20.ipynb) |
| The heatmaps shows the nucleosome density estimated by SeATAC (blue) and NucleoATAC (purple) on a 1% down-sampled dataset. | Figure 3b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/GM12878_nucleosome_calling_f3%20.ipynb) |
| The violin plot shows the AUC (area under ROC) of SeATAC and NucleoATAC on 523 ATAC-seq samples from 20 studies. *** Wilcoxon rank sum test p-value < 0.001. | Figure 3c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/summarize_comp.ipynb) |
| The AUC of SeATAC and NucleoATAC at different read counts cutoff from 1 to 20 (the minimum reads in a V-plot). | Figure 3d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/summarize_comp.ipynb) |

### Figure 4
|  | Figures | Link | 
| --- | --- | --- | 
| The ROC curve for detecting nucleosome changes from ATAC-seq with 10% of the sequencing reads from the full dataset (GM12878). | Figure 4a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/GM12878_diff_nuc_f4ac.ipynb) |
| The raw and estimated V-plot of a NFR (chr1:113162059-113162698) and a NOR (chr2:226653061-226653700) region are shown | Figure 4b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/GM12878_diff_nuc_f4ac.ipynb) |
| The heatmaps show the nucleosome density of ~5,000 sampled NOR and NFR regions estimated by SeATAC & NucleoATAC  on a 10% down-sampled dataset and NucleoATAC signal on the full dataset (black) & a MNase-seq dataset on GM12878. |  Figure 4c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/GM12878_diff_nuc_f4ac.ipynb) |
| The violin plot shows the AUC (area under ROC) of SeATAC and NucleoATAC on 523 ATAC-seq samples from 20 studies. *** Wilcoxon rank sum test p-value < 0.001. |  Figure 4d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/summarize_comp.ipynb) |
| The AUC of SeATAC and NucleoATAC at different read counts cutoff from 1 to 20 (the minimum reads in a V-plot). |  Figure 4e | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/summarize_comp.ipynb) |

### Figure 5
|  | Figures | Link | 
| --- | --- | --- | 
| The Venn diagrams show the number of Etv2 motifs with increased chromatin accessibility identified by SeATAC, MACS2 and NucleoATAC Etv2 induced MEF. | Figure 5a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_Etv2_MEF_and_EB_v0_4_0_pathway_analysis_f5.ipynb) |
| The Venn diagrams show the number of Etv2 motifs with increased chromatin accessibility identified by SeATAC, MACS2 and NucleoATAC Etv2 induced EB differentiation | Figure 5b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_Etv2_MEF_and_EB_v0_4_0_pathway_analysis_f5.ipynb) |
| The aggregated V-plot includes 1,626, 222 and 2,305 Etv2 motifs with increased chromatin accessibility identified by SeATAC only, MACS2 only and NucleoATAC only in ATAC-seq data of Etv2 induced EB differentiation | Figure 5c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_Etv2_EB_v0_4_0_Vplots_for_and_EBs_Figure.ipynb) |
|  The barplots show the Gene Ontology (GO) terms that are significantly associated with the genes which promoters (-5,000 - +1,000bp region flanking the TSS) have Etv2 motifs with increased chromatin accessibility, identified by SeATAC, MACS2 and NucleoATAC. | Figure 5d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_Etv2_MEF_and_EB_v0_4_0_pathway_analysis_f5.ipynb) |

### Figure 6
|  | Figures | Link | 
| --- | --- | --- | 
| Dot plots comparing the changes of motif associated chromatin accessibility estimated by chromVAR (x-axis) and the difference of the percent of TFBS with decreased or increased chromatin accessibility estimated by SeATAC. | Figure 6a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Etv2_MEF_EB_motifs.ipynb) |
| The barplots show the genomic distribution of Etv2 binding sites with decreased (NFR->NOR) or increased (NOR->NFR) chromatin accessibility in EB differentiation or MEF reprogramming. | Figure 6b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Etv2_MEF_EB_Etv2_v1.ipynb) |
| The aggregated V-plot include 3,000 and 1,623 Etv2 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during MEF reprograming. | Figure 6c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Etv2_MEF_EB_Etv2_v1.ipynb) |
| The heatmaps showing Etv2, Brg1, H3K27ac ChIP-seq of 3,000 and 1,623 Etv2 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility at day 2.5 EB (Brg1 and H3K27ac), 3 hours post Etv2 induction (Etv2), and 12 hours post Etv2 induction (Etv2, Brg1 and H3K27ac). | Figure 6d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Etv2_MEF_EB_Etv2_v1.ipynb) |
| The barplots show the percent of genes that were down-regulated, up-regulated or not changed between day 2.5 EB and 12 hours post Etv2 induction. | Figure 6e | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/EB_RNA_and_NOR_NFR_f6ef.ipynb) |
| Brachyury (T) and Mycn are significantly down-regulated during the Etv2 induced differentiation. | Fgure 6f | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/EB_RNA_and_NOR_NFR_f6ef.ipynb) |
| Brachyury (T) and Mycn (f) have Etv2 motifs that become significantly less accessible during the differentiation at their promoter region (-5,000 - +1,000bp region flanking the TSS) | Figure 6g | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Vplots_for_and_EBs_specific_genes.ipynb) |

## Supplementary Figures


### Figure S1
|  | Figures | Link | 
| --- | --- | --- |
| The density plots show the observed (red) and corrected (green) fragment size distribution of 13 samples from a human hematopoietic differentiation ATAC-seq data (GSE96771). | Figure S1a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_corrects_batch_effects_sf1.ipynb) |

### Figure S2
|  | Figures | Link | 
| --- | --- | --- |
| The plot shows the AUC of SeATAC, NucleoATAC and MACS2 at different shift sizes (from 10 to 100) used to generate the synthetic data for evaluating task #1. | Figure S2a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/seatac_GM12878_task1.ipynb) |

### Figure S3
|  | Figures | Link | 
| --- | --- | --- |
| The plots show the AUC (area under ROC) of SeATAC on 523 ATAC-seq samples from 20 studies at (a) total read counts (Total QNAMEs), (b) mitochondria rate, (c) proper pair rate, (d) unmapped rate, (e) has unmapped mate rate, (f) non-redundant fraction, (g) PCR bottleneck coefficient 1, and (h) PCR bottleneck coefficient 2. | Figure S3a-h | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/summarize_comp.ipynb) |

### Figure S4
|  | Figures | Link | 
| --- | --- | --- |
| The area under ROC (AUC) of three tools, SeATAC, NucleoATAC and MACS2 on the regions over promoter region (column wise) and latent dimensions (row wise). | Figure S4b | [R](https://github.com/gongx030/seatac_manuscript/blob/main/notebooks/pa_summary.ipynb) |
| The area under ROC (AUC) of three tools on 17 paired RNA-seq / ATAC-seq datasets. | Figure S4c | [R](https://github.com/gongx030/seatac_manuscript/blob/main/notebooks/pa_summary.ipynb) |

### Figure S5
|  | Figures | Link | 
| --- | --- | --- |
| The aggregated V-plot includes: 728 and 1,633 NFKB1 binding sites with increased chromatin accessibility in GM12878 compared with K562 at distal and promoter regions, respectively. The heatmap color indicates the estimated read density. | Figure S5a | [R](https://github.com/gongx030/seatac_manuscript/blob/main/notebooks/K562_vs_GM12878.ipynb) |
| The line plots include: mean signal of H3K27ac, h3K4me1, H3K4me3 signals of 728 and 1,633 NFKB1 binding sites with increased chromatin accessibility in GM12878 compared with K562 at distal and promoter regions. | Figure S5b | [R](https://github.com/gongx030/seatac_manuscript/blob/main/notebooks/K562_vs_GM12878.ipynb) |
| The mean squared error of observed and predicted histone modification signals. | Figure S5d | [R](https://github.com/gongx030/seatac_manuscript/blob/main/notebooks/pred_histone_bs640_k10.ipynb) |

### Figure S6
|  | Figures | Link | 
| --- | --- | --- |
| The aggregated V-plot includes 2,776, 116 and 1,449 Etv2 motifs with increased chromatin accessibility identified by SeATAC only, MACS2 only and NucleoATAC only in ATAC-seq data of Etv2 induced MEF reprogramming | Figure S6a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/SeATAC_Etv2_MEF_v0_4_0_Vplots_for_and_MEFs_Figure.ipynb) |
| The heatmaps show the Etv2, Brg1, H3K27ac ChIP-seq of 3,996 and 1,307 Etv2 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility at undifferentiated MEFs (Brg1 and H3K27ac), 1 day post-Etv2 induction (Etv2), and 7 days post-Etv2 induction (Etv2, Brg1 and H3K27ac). | Figure S6b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/Etv2_MEF_EB_Etv2_v1.ipynb)| 
| The UCSC genome browser track show the ATAC-seq density near the Etv2 motifs at the promoters of Brachyury (T) and Mycn. | Figure S6c | [T](https://genome.ucsc.edu/s/ndsouza/T_new) <br> [Mycn](https://genome.ucsc.edu/s/ndsouza/Mycn_new) |

### Figure S7
|  | Figures | Link | 
| --- | --- | --- |
| The Venn diagrams show the number of Ascl1 motifs with increased chromatin accessibility identified by SeATAC, MACS2 and NucleoATAC. | Figure S7a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_Ascl1_MEFs_D22_analysis_sf3.ipynb) |
| The barplots show the Gene Ontology (GO) terms that are significantly associated with the genes which promoters (-5,000 - +1,000bp region flanking the TSS) have Ascl1 motifs with increased chromatin accessibility, identified by SeATAC, MACS2 and NucleoATAC.  | Figure S7b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_Ascl1_MEFs_D22_analysis_sf3.ipynb) |
| The aggregated V-plot includes 8,658, 7,687 and 7,708 Ascl1 motifs with increased chromatin accessibility identified by SeATAC only, MACS2 only and NucleoATAC only in ATAC-seq data of Ascl1 induced MEF reprogramming (undifferentiated MEFs vs. 22 days post Ascl1 induction). | Figure S7c |  [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_Ascl1_MEFs_D22_analysis_sf3.ipynb) |

### Figure S8
|  | Figures | Link | 
| --- | --- | --- |
| The Venn diagrams show the number of OSK motifs with increased chromatin accessibility identified by SeATAC, MACS2 and NucleoATAC. | Figure S8a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_OSK_MEFs_D7_sf4.ipynb) |
| The barplots show the Gene Ontology (GO) terms that are significantly associated with the genes which promoters (-5,000 - +1,000bp region flanking the TSS) have OSK motifs with increased chromatin accessibility, identified by SeATAC, MACS2 and NucleoATAC. | Figure S8b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_OSK_MEFs_D7_sf4.ipynb) |
| The aggregated V-plot includes 5,826, 1,355 and 6,371 OSK motifs with increased chromatin accessibility identified by SeATAC only, MACS2 only and NucleoATAC only in ATAC-seq data of OSK induced MEF reprogramming | Figure S8c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_OSK_MEFs_D7_sf4.ipynb) |

### Figure S9
|  | Figures | Link | 
| --- | --- | --- |
| The dot plots compare the changes of motif associated chromatin accessibility estimated by chromVAR (x-axis) and the difference of the percent of TFBS with decreased or increased chromatin accessibility estimated by SeATAC | Figure S9a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Ascl1_MEF_motifs.ipynb) |
| The barplots show the genomic distribution of Ascl1 binding sites with decreased (NFR->NOR) or increased (NOR->NFR) chromatin accessibility in MEF reprogramming. | Figure S9b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Ascl1_MEF_Seatac_Supplementary_v1.ipynb) |
| The aggregated V-plot include 24,098 and 7,071 Ascl1 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during MEF reprograming. | Figure S9c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Ascl1_MEF_Seatac_Supplementary_v1.ipynb) |
| The heatmaps show the MNase-seq, H3K27m3, H3K36m3, H3K9ac, H3K79me2, H3K4me2, H3K4me1 and P300 ChIP-seq signals in undifferentiated MEFs of 24,098 and 7,071 Ascl1 binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during the MEF reprogramming. | Figure S9d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Ascl1_MEF_Seatac_Supplementary_v1.ipynb) |
| The V-plot show Ascl1 motifs with decreased chromatin accessibility at the promoters (-5,000 - +1,000bp region flanking the TSS) of four genes (Hmga2, Elf4, Egfr and Hes1) that are down-regulated during the Ascl1 induced MEF reprogramming. | Figure S9e | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_Ascl1_MEFs_D22_specific_genes_sf5e.ipynb) |

### Figure S10
|  | Figures | Link | 
| --- | --- | --- |
| The dot plots compare the changes of motif associated chromatin accessibility estimated by chromVAR (x-axis) and the difference of the percent of TFBS with decreased or increased chromatin accessibility estimated by SeATAC | Figure S10a | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/OSK_MEF_motifs.ipynb) |
| The barplots show the genomic distribution of OSK binding sites with decreased (NFR->NOR) or increased (NOR->NFR) chromatin accessibility in MEF reprogramming. | Figure S10b | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/OSK_MEF_Seatac_Supplementary.ipynb) |
| The aggregated V-plot include 15,825 and 4,935 OSK binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during MEF reprograming. | Figure S10c | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/OSK_MEF_Seatac_Supplementary.ipynb) |
| The heatmaps show the MNase-seq, H3K27m3, H3K36m3, H3K9ac, H3K79me2, H3K4me2, H3K4me1 and P300 ChIP-seq signals in undifferentiated MEFs of 15,825 and 4,935 OSK binding sites that have increased (NOR->NFR) or decreased (NFR->NOR) chromatin accessibility during the MEF reprogramming. | Figure S10d | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/OSK_MEF_Seatac_Supplementary.ipynb) |
| The barplots show the percent of genes that were down-regulated, up-regulated or not changed between undifferentiated MEFs and 7 hours post OSK induction. | Figure S10e | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/OSK_RNA_and_NOR_NFR_sf6ef.ipynb) |
| Maf and Smad3 are significantly down-regulated during the OSK induced MEF reprogramming. | Figure S10f | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/OSK_RNA_and_NOR_NFR_sf6ef.ipynb)  |
| Maf and Smad3 have OSK motifs that become significantly less accessible during the differentiation at their promoter region (-5,000 - +1,000bp region flanking the TSS). | Figure S10g | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/SeATAC_OSK_MEFs_D7_specific_genes_sf6g.ipynb) |

### Figure S11
|  | Figures | Link | 
| --- | --- | --- |
| Example regions with significantly increased chromatin accessibility from undifferentiated MEFs to D7 Flk1+ samples. (f-j) Example regions with significantly decreased chromatin accessibility from undifferentiated MEFs to D7 Flk1+ samples. | Figure S11a-j | [R](https://colab.research.google.com/github/gongx030/seatac_manuscript/blob/main/notebooks/Etv2_MEF_histone.ipynb) |


