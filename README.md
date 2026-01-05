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

### Figure 3. 
#### Box plot of all clusters divided by condition. Include statistical comparison information.

```
## Performing logit transformation of proportions
```

```
## group variable has > 2 levels, ANOVA will be performed
```

![](README_files/figure-html/boxplot-1.png)<!-- -->

### Figure 4. 
#### UMAP. Reclustering of only tumor cell clusters. Colored by cluster ID.
![](README_files/figure-html/load_tumor_only-1.png)<!-- -->



### Figure 5. 
#### Pseudotime trajectory analysis of above tumor cell clustering (to define undifferentiated vs differentiated clusters).
![](README_files/figure-html/pseudotime-1.png)<!-- -->

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

Built with R 4.5.2.
