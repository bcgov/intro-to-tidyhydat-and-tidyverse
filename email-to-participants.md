Text available at: https://github.com/bcgov/intro-to-tidyhydat-and-tidyverse/blob/master/email-to-participants.md

**Is this workshop for me?**

Do you have any experience with R? If the answer is no, don't worry. This workshop is designed for people with little to no experience with R but are interested in bringing reproducible analysis to their hydrological data analysis needs. 

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

Open R and paste the following code into the blinking console to install required R packages and download the HYDAT database:
    
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

**What should I do if I have problem?**
Email me! I am happy to sort of R installation issues, HYDAT downloading issues, package library locations or whatever other weird installation problems you may have ***before the workshop***. If we can solve these problems beforehand, we will be able to squeeze in much more actual R work during our time together. 

If you have any other questions, feel free to email me. 



