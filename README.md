# input_select-variables

A shiny app for the following `ggvis` example of how to use `input_select()` in a `shiny` app.

```r
library(dplyr)
library(ggvis)
iris %>% 
  ggvis(x = input_select(c('Petal.Width', 'Sepal.Length'), map = as.name)) %>% 
  layer_points(y = ~Petal.Length, fill = ~Species)
```
