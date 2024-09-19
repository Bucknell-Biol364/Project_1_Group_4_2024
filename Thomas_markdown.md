Thomas_section
================
2024-09-19

``` r
penguins <- read.csv("palmerpenguins_extended.csv")
```

``` r
install.packages("viridis")
```

    ## Warning: package 'viridis' is in use and will not be installed

``` r
library(viridis)


ggplot(penguins) +
  aes(x = bill_length_mm, y = bill_depth_mm, color = body_mass_g) +
  geom_point() + 
  scale_color_viridis("body_mass_g", option="viridis") +
  theme_classic()
```

![](Thomas_markdown_files/figure-gfm/INSTALLING%20VIRIDIS%20+%20GRAPH%20Example-1.png)<!-- -->

``` r
#Note that you have to use the "scale_color_viridis_d("") command if you want 
#to use viridis with discrete variables.
#Options are "magma" (or "A") "inferno" (or "B") "plasma" (or "C") 
#"viridis" (or "D") "cividis" (or "E") "rocket" (or "F") "mako" (or "G") and 
# "turbo" (or "h"). We should decide on a consistent one together. 
```

\#git config pull.rebase false - can use dropdown on pull menu to pull
with \#rebase automatically \#We can make branches off the project to
prevent conflicts until the end \## Guidelines: \#pull before starting
to work/edit
