## this is a markdown file

# Density ridgeline plots

#references

Plot One Variable: Frequency Graph, Density Distribution and More

*link*

http://www.sthda.com/english/articles/32-r-graphics-essentials/133-plot-one-variable-frequency-graph-density-distribution-and-more/


# Density ridgeline plots

```{r}
install.packages("ggridges")

library(ggplot2)
library(ggridges)
theme_set(theme_ridges())

ggplot(iris, aes(x = Sepal.Length, y = Species)) +
  geom_density_ridges(aes(fill = Species)) +
  scale_fill_manual(values = c("#00AFBB", "#E7B800", "#FC4E07"))
```
