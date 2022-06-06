# Making a relative abundance barplot with ggplot2

This repository contains the materials and code required to create
a relative abundance barplot as described in this
[video](https://www.youtube.com/watch?v=siIoupAnILk).

The data plotted corresponds to bacterial abundance that live in the soil,
rhizospher (R) and endophytic compartment (E) of *Arabidopsis thaliana*
plants. The data is a small subset of the dataset that was published
[here](https://www.nature.com/articles/nature11237).

These materials were created for the 2022 SFSU
[Science Coding Immersion Program (SPIC)](https://sfsuscip.wixsite.com/scip) &
[Promoting Inclusivity in Computing (PINC)](https://pinc.sfsu.edu/pinc/pinc/bdsp)
summer pograms.

## What do you need?

In order to follow this tutorial you just need [R](https://cran.r-project.org/)
with the [tidyverse](https://www.tidyverse.org/) package installed.
If you haven't installed the tidyverse yet, simply open an R session and type:

```r
install.packages("tidyverse")
```

It is also recommended to have [RStudio](https://www.rstudio.com/) installed
although you can use any platfform that allows you to run R code.

### The data

The code in the [video](https://www.youtube.com/watch?v=siIoupAnILk)
and the [extended example](extended_example.md) requires the three files in
the subdirectory [data/rhizo](data/rhizo). Those files correspond to
the OTU table, the OTU taxonomy, and the sample metadata and they must be
in the machine where you are running the R code.

There is additional files in the [data/hmp_v13](data/hmp_v13) subdirectory.
The files there have the same names as the files in [data/rhizo](data/rhizo),
but correspond instead to a subset of the data from the Human Microbiome
Project. The data in these files was downloaded from
[this repository](https://hmpdacc.org/hmp/HMQCP/) and the files are formatted
so that they will match the format of the rhizospher dataset. Thus, these
files can be analyzed with the  same code in order to explore
a different host-microbe system.

## Extended example & excercises

The extended example provides additional details about the code and
data used in the workshop. The extended example is in the file
[extended_example.md](extended_example.md). The RMarkdown code that generated
that filee is at [extended_example.Rmd](extended_example.Rmd)

Hera are some additional excerscises that you can do to practive what
you learned in this workshop:

1. You learned how to sort the taxonomic groups in the barplot,
can you sort the samples by relative Proteobacteria abundance?
can you reverse the order of the facets?

2. Look a the extra files at [data/hmp_v13](data/hmp_v13). Can you
make a plot showing the bacterial taxonomic distributions in human stool
and Saliva, are there any differences by sex?

## More resources

* For any questions just [raise an issue](https://github.com/surh/scip_barplot/issues) in this repository

* [Slides](slides/2022_SCIP_video.pdf) from the workshop video.

* [Video](https://www.youtube.com/watch?v=siIoupAnILk) of the workshop.

## License & copyright

(C) Copyright 2022 Sur Herrera Paredes

[![Creative Commons License](https://i.creativecommons.org/l/by-nc/4.0/88x31.png)](LICENSE)

This work is licensed under a
[Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/).
