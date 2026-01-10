---
title: "oligo_project"
output: 
  html_document:
    keep_md: true
date: "2025-12-26"
---

***
# Test plots for oligo project








## UMAP plots 
### Figure 1
#### UMAP colored by cluster.
![](README_files/figure-html/umap_labeled-1.png)<!-- -->

### Figure 2
#### UMAP colored by condition.
![](README_files/figure-html/umap_by_tumor-1.png)<!-- -->

#### Heatmap
#### GSEA - heatmap
#### Microglia / macrophage differences
#### QC

### Figure 3. 
#### Box plot of all clusters divided by condition. Include statistical comparison information.

```
## Performing logit transformation of proportions
```

```
## group variable has > 2 levels, ANOVA will be performed
```

![](README_files/figure-html/boxplot-1.png)<!-- -->

***

## Tumor only
### Figure 4. 
#### UMAP. Reclustering of only tumor cell clusters. Colored by cluster ID.
![](README_files/figure-html/load_tumor_only-1.png)<!-- -->

### Split by condition 

```
## $Oligo_Cdkn2a
```

![](README_files/figure-html/tumor_only_split-1.png)<!-- -->

```
## 
## $IDH_WT_GBM
```

![](README_files/figure-html/tumor_only_split-2.png)<!-- -->

```
## 
## $Oligo_Trp53
```

![](README_files/figure-html/tumor_only_split-3.png)<!-- -->

```
## 
## $Normal_Brain
```

![](README_files/figure-html/tumor_only_split-4.png)<!-- -->

## Trajectory inference using Monocle3
### Figure 5. 
#### Pseudotime trajectory analysis of above tumor cell clustering (to define undifferentiated vs differentiated clusters).
![](README_files/figure-html/pseudotime-1.png)<!-- -->

#### Differential expression as a function of pseudotime

### Figure 6. 
#### Box plot of tumor cell clusters only divided by condition. Include statistical comparison information.

```
## Performing logit transformation of proportions
```

```
## group variable has > 2 levels, ANOVA will be performed
```

![](README_files/figure-html/tumor_boxplot-1.png)<!-- -->

***
## Heatmap
### By cell

![](README_files/figure-html/heatmap-1.png)<!-- -->

### By cluster
#### Scaled - restrict to just tumor clusters for main figure; can have all for supplemental
![](README_files/figure-html/heatmap_mean_scaled-1.png)<!-- -->

#### Midpoint 0
![](README_files/figure-html/heatmap_mean-1.png)<!-- -->

***

## GSEA

```
## [1] "Under construction."
```


Built with R 4.5.2.
