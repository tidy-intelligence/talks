# 2024-01-01 BRUG

## Set-up

These are the steps that I executed to set up this project:

1. `install.packages("renv")`
2. `renv::activate()`
3. `install.packages("reticulate")`
4. `reticulate::install_python(version="3.10.11", force = TRUE)`
5. Tell `renv` to use python: 
 - On Windows: `renv::use_python(paste0("C:/Users/", Sys.info()["user"], "/AppData/Local/r-reticulate/r-reticulate/pyenv/pyenv-win/versions/3.10.11/python.exe"))`
 - On Mac: `renv::use_python("~/.pyenv/versions/3.10.11/bin/python")`
6. `renv::snapshot()`
