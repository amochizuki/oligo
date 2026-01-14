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

***

## Tumor only
### Figure 4. 
#### UMAP. Reclustering of only tumor cell clusters. Colored by cluster ID.
![](README_files/figure-html/load_tumor_only-1.png)<!-- -->

### Split by condition 


## Trajectory inference using Monocle3
### Figure 5. 
#### Pseudotime trajectory analysis of above tumor cell clustering (to define undifferentiated vs differentiated clusters).
![](README_files/figure-html/pseudotime-1.png)<!-- -->

#### Differential expression as a function of pseudotime
##### Used genes with q value < 0.01 differential expression analysis (total n = 14,037) - can use others
![](README_files/figure-html/pt_de-1.png)<!-- -->

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
#### Scaled


#### pheatmap

![](README_files/figure-html/pheatmap_mean_scaled-1.png)<!-- -->
#### Midpoint 0
![](README_files/figure-html/heatmap_mean-1.png)<!-- -->

***

## GSEA


![](README_files/figure-html/GSEA_heatmap-1.png)<!-- -->

#### Microglia / macrophage differences
##### Oligo Cdkn2a vs normal brain

```
## $plot
```

![](README_files/figure-html/mg_mph_cdkn2a_vs_nl-1.png)<!-- -->

```
## $plot
```

![](README_files/figure-html/mg_mph_cdkn2a_vs_nl-2.png)<!-- -->

##### Oligo Trp53 vs normal brain

```
## $plot
```

![](README_files/figure-html/mg_mph_p53_vs_nl-1.png)<!-- -->

```
## $plot
```

![](README_files/figure-html/mg_mph_p53_vs_nl-2.png)<!-- -->

##### IDH WT GBM vs normal brain

```
## $plot
```

![](README_files/figure-html/mg_mph_gbm_vs_nl-1.png)<!-- -->

```
## $plot
```

![](README_files/figure-html/mg_mph_gbm_vs_nl-2.png)<!-- -->

#### Trailmaker QC settings
<table>
 <thead>
  <tr>
   <th style="text-align:left;">   </th>
   <th style="text-align:left;"> classifier </th>
   <th style="text-align:left;"> cellSizeDistribution </th>
   <th style="text-align:left;"> mitochondrialContent </th>
   <th style="text-align:left;"> numGenesVsNumUmis </th>
   <th style="text-align:left;"> doubletScores </th>
   <th style="text-align:left;"> dataIntegration </th>
   <th style="text-align:left;"> configureEmbedding </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> TIM055 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 91892 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005938702 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.0001132759 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4450093 </td>
   <td style="text-align:left;"> analysisTool = scanpy, method = harmony, numGenes = 2000, normalisation = logNormalize, method = rpca, numPCs = 30 </td>
   <td style="text-align:left;"> method = umap, distanceMetric = cosine, minimumDistance = 0.3, method = leiden, resolution = 0.8 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM056 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 88852 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005417118 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.00009344048 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4237304 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM057 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 52661 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.01593528 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.00009119927 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4759446 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM058 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 53079 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.01356374 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.000114771 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4521705 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM059 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 151633 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005409603 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.00008873114 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4872152 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM060 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 197965 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005328189 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.0001004823 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.3814495 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM061 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 81950 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005609059 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.001 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.3727773 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM062 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 81265 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005952935 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.0001129944 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.3910435 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM063 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 98004 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.00520047 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.00008002561 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4747944 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM064 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 60287 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005415162 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.0001237777 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4484248 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM065 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 96917 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005557575 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.0001085187 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.3973176 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM066 </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 88152 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005331363 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.00009521996 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4022901 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM045X </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 72052 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.006008584 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.00007392076 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.3469654 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM046X </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 75486 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005730428 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.00007785737 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4371886 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM047X </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 61277 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005298013 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.000101688 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.441427 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
  <tr>
   <td style="text-align:left;"> TIM048X </td>
   <td style="text-align:left;"> FDR = 0.01 </td>
   <td style="text-align:left;"> binStep = 200, minCellSize = 74047 </td>
   <td style="text-align:left;"> method = absoluteThreshold, binStep = 0.3, maxFraction = 0.005293246 </td>
   <td style="text-align:left;"> regressionType = spline, p.level = 0.0001007252 </td>
   <td style="text-align:left;"> binStep = 0.02, probabilityThreshold = 0.4360736 </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
  </tr>
</tbody>
</table>

Built with R 4.5.2.
