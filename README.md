# SPIDDOR
Modeling, simulation and analysis of Boolean networks applied to Systems Pharmacology.

## To install SPIDDOR:  
```{r}
install.packages("devtools")  
library(devtools)  
install_github("SPIDDOR/SPIDDOR") 
```
If you use a proxy server you need to install httr package and then:
```{r}
library(httr)
#Set your proxy here:
set_config(use_proxy("10.10.10",8080))
install_github("SPIDDOR/SPIDDOR") 
```
Additionally, Rtools is needed to use the simulation algorithm in C++. 
## To install Rtools:  
You can download it from https://cran.r-project.org/bin/windows/Rtools/ .   
Select the Rtools download compatible with your R version. We recommend that users use the latest release of Rtools with the latest release of R. Be aware of the path where Rtools or RBuildTools is installed and use the Connect2Rtools function each time you start a new R session in order to connect the package with Rtools gcc compiler (only for Windows users). Example:  
```{r}
library(SPIDDOR)  
Connect2Rtools(path="C:\\Rtools")
```

