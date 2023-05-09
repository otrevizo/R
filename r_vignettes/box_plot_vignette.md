---
title: "Scatter plot vignette"
output:
  html_document:
    toc: yes
    keep_md: yes
  pdf_document:
    toc: yes
  github_document:
    toc: yes
---




# Bar plot vignette

Based on Dr. Bharatendra https://www.youtube.com/watch?v=BPR_Dkll17Y&list=PL34t5iLfZddtUUABMikey6NtL05hPAp42&index=8 

Done here for learning purposes.

# Basic

## Example 1


```r
ggplot(possum, aes(x=factor(site), y=taill)) +
  geom_boxplot()
```

![](box_plot_vignette_files/figure-html/unnamed-chunk-1-1.png)<!-- -->

## Example 2


```r
ggplot(possum, aes(x=sex, y=chest, col=sex)) +
  geom_boxplot()
```

![](box_plot_vignette_files/figure-html/unnamed-chunk-2-1.png)<!-- -->


## With interaction


```r
ggplot(possum, aes(x=interaction(sex, site), y=chest, col=sex, fill=sex)) +
  geom_boxplot(color='black')
```

![](box_plot_vignette_files/figure-html/unnamed-chunk-3-1.png)<!-- -->



