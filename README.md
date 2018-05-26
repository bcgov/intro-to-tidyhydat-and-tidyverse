<div id="devex-badge"><a rel="Exploration" href="https://github.com/BCDevExchange/docs/blob/master/discussion/projectstates.md"><img alt="Being designed and built, but in the lab. May change, disappear, or be buggy." style="border-width:0" src="https://assets.bcdevexchange.org/images/badges/exploration.svg" title="Being designed and built, but in the lab. May change, disappear, or be buggy." /></a></div>

# Introduction to R and the tidyverse in Hydrology

This is the repo for *Introduction to R and the tidyverse in Hydrology* to be delivered at the [Canadian Water Resources Association](https://conference.cwra.org/) 2018 conference in Victoria, British Columbia on May 28, 2018. The workshop repo is currently under development and all materials should be considered a work in progress.

This is a 4 hour hands-on workshop that leans heavily on the book [R for Data Science](http://r4ds.had.co.nz/) and on the [tidyhydat](https://CRAN.R-project.org/package=tidyhydat) package. This workshop is intended as an introduction for people interested in hydrological analysis and who would like to try using R. In this workshop you will learn how to:

- Recognize basic elements of the R programming language
- Use the R package tidyhydat to access realtime and historical Water Survey of Canada data directly from R
- Conduct a variety basic data tidying steps
- Generate high quality plots in R
- Understand where and how to seek help for R
- Take away your R recipes for future analysis

You will learn how to visualize and transform untidy data formats. Along the way, you will learn and use several packages from the tidyverse including ggplot2, dplyr, tidyr, and purrr. In addition, we will make use of the tidyhydat package, which imports and tidies [Water Survey of Canada](https://wateroffice.ec.gc.ca/index_e.html) hydrometric data into R.



## Software requirements
You will need a working installation of R and RStudio available from here:

Install R from here:
https://cloud.r-project.org/

Install RStudio from here:
https://www.rstudio.com/products/rstudio/download/#download

You'll need the following packages:

```R
install.packages(c("tidyverse", "tidyhydat", "usethis", "rmarkdown"))
```

Then you can grab a local copy of all the slides, code and data:

```R
usethis::use_course("https://bit.ly/2L95hCb")
```

To get back to this project later, double-click on "intro-to-tidyhydat-and-tidyverse.Rproj".

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a>

<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Original repo *Data Science in the tidyverse*</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/cwickham/data-science-in-tidyverse" property="cc:attributionName" rel="cc:attributionURL">Charlotte Wickham</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.  Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/rstudio/master-the-tidyverse" rel="dct:source">https://github.com/rstudio/master-the-tidyverse</a>.

## Acknowledgements

I have forked this repo from [Hadley Wickham](https://github.com/hadley/data-science-in-tidyverse) who in turn forked it from [Charlotte Wickham](https://github.com/cwickham/data-science-in-tidyverse), who forked it from [RStudio](https://github.com/rstudio/master-the-tidyverse). The feel, look and flow of the material in this workshop was originally created by these authors. My main contribution was adapt the examples to hydrologically based data. Huge thanks to [Hadley](http://hadley.nz/), [Charlotte](http://cwick.co.nz) and [Garrett](https://github.com/garrettgman) for creating the slides and accompanying materials!
