packages <- c("admiral", "dplyr", "ggplot2", "tidyverse","haven", "readxl", "survminer", "survival")  

for (pkg in packages) {
  if (!require(pkg, character.only = TRUE)) {
    install.packages(pkg, dependencies = TRUE)
    library(pkg, character.only = TRUE)
  }
}
