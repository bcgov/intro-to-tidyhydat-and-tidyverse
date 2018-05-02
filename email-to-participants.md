*(This will be sent to registered particpants by email, but I'm also posting here as a convenient place to field any questions/issues.)*


**What should you bring?**
 - Laptop installed with R and RStudio


**Is this class for me?**

This class is designed for people who no experience with R but are interested in applying it to their hydrological data analysis needs. 

**Is there anything you should do before arriving?**

Yes!

Install R and RStudio

If you are dying to get started, feel free to poke around the materials on [github](https://github.com/bcgov/intro-to-tidyhydat-and-tidyverse)

If you have any other questions, feel free to email me. 

**Packages to install before** arriving:
Enter these four lines of code and paste the output in an email to me (It should say [1] TRUE TRUE TRUE):

```
.libPaths()

pkgs <- c("tidyverse","tidyhydat","rmarkdown")
install.packages(pkgs)
install_success <- pkgs %in% rownames(installed.packages())

if(any(!install_success)){
  miss_pkgs <- pkgs[which(!install_success)]
  cat("The following packages were not successfully installed:", paste0(miss_pkgs, collapse = ", "))
}


did_it_work <- tidyhydat::download_hydat()
if(isTRUE(!did_it_work)) cat("HYDAT did not download successfully")
```





