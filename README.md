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

### Split by condition - re-integrated

```
## [[1]]
```

![](README_files/figure-html/tumor_only_split-1.png)<!-- -->

```
## 
## [[2]]
```

![](README_files/figure-html/tumor_only_split-2.png)<!-- -->

```
## 
## [[3]]
```

![](README_files/figure-html/tumor_only_split-3.png)<!-- -->

```
## 
## [[4]]
```

![](README_files/figure-html/tumor_only_split-4.png)<!-- -->

### Alternative dimension reduction - ForceAtlas2
![](README_files/figure-html/forceatlas2-1.png)<!-- -->



## Trajectory inference using PAGA and DPT
### Figure 5. 
#### Pseudotime trajectory analysis of above tumor cell clustering (to define undifferentiated vs differentiated clusters).
![](README_files/figure-html/pseudotime-1.png)<!-- -->

![](README_files/figure-html/pseudotime_FA-1.png)<!-- -->


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



### By cluster
#### Scaled - restrict to just tumor clusters for main figure; can have all for supplemental
![](README_files/figure-html/heatmap_mean_scaled-1.png)<!-- -->

#### Midpoint 0
![](README_files/figure-html/heatmap_mean-1.png)<!-- -->

***

## GSEA


Built with R 4.5.2.
