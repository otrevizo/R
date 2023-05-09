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

## Vertical (default)


```r
ggplot(possum, aes(x=factor(site), y=taill)) +
  geom_col()
```

![](bar_plot_vignette_files/figure-html/unnamed-chunk-1-1.png)<!-- -->

## Horizontal



```r
ggplot(possum, aes(x=factor(site), y=taill)) +
  geom_col() +
  coord_flip()
```

![](bar_plot_vignette_files/figure-html/unnamed-chunk-2-1.png)<!-- -->




```r
ggplot(possum, aes(x=factor(site), y=taill, fill=factor(site))) +
  geom_col() +
  coord_flip()
```

![](bar_plot_vignette_files/figure-html/unnamed-chunk-3-1.png)<!-- -->
