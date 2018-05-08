*(This will be sent to registered particpants by email, but I'm also posting here as a convenient place to field any questions/issues.)*


**Is this class for me?**

Do you have any expereince with R? If no don't worry. This class is designed for people who have no experience with R but are interested in applying it to their hydrological data analysis needs. 

**What should you bring?**
 - Laptop installed with R and RStudio that is capable of connecting to Wifi
 
**Considerations**
- You have administrative access to your computer
- All software and packages should be installed on your computer rather than a network drive
 

**Is there anything you should do before arriving?**

Yes! Four things. 

Install R from here:
https://cloud.r-project.org/

Install RStudio from here:
https://www.rstudio.com/products/rstudio/download/#download

Open R and paste the following code into the blinking console:
    ```
    
    .libPaths()
    
    pkgs <- c("tidyverse","tidyhydat","rmarkdown","usethis")
    install.packages(pkgs)
    install_success <- pkgs %in% rownames(installed.packages())
    
    if(any(!install_success)){
      miss_pkgs <- pkgs[which(!install_success)]
      cat("The following packages were not successfully installed:", paste0(miss_pkgs, collapse = ", "))
    }
    
    
    did_it_work <- tidyhydat::download_hydat()
    if(isTRUE(!did_it_work)) cat("HYDAT did not download successfully")
    ```

This code will take about 10 to fifteen minutes to run.

**The course itself**

If you are dying to get started, feel free to poke around the materials on [github](https://github.com/bcgov/intro-to-tidyhydat-and-tidyverse)

If you have any other questions, feel free to email me. 



