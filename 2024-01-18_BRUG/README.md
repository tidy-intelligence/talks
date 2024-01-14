# 2024-01-01 BRUG

## References

I used the following resources to compile this talk:

- "Hello, Quarto" slides by Julia Lowndes and Mine Çetinkaya Rundel, presented at RStudio Conference 2022: https://mine.quarto.pub/hello-quarto/
- "From Jupyter Notebooks to websites with Quarto" slides by Mine Çetinkaya Rundel, presented at PyData 2023: https://mine.quarto.pub/quarto-pydata/#/title-slide


## Set-up for R and Python

These are the steps that I executed to set up this project:

1. `install.packages("renv")`
2. `renv::activate()`
3. `install.packages("reticulate")`
4. `reticulate::install_python(version="3.10.11", force = TRUE)`
5. Tell `renv` to use python: 
 - On Windows: `renv::use_python(paste0("C:/Users/", Sys.info()["user"], "/AppData/Local/r-reticulate/r-reticulate/pyenv/pyenv-win/versions/3.10.11/python.exe"))`
 - On Mac: `renv::use_python("~/.pyenv/versions/3.10.11/bin/python")`
6. `renv::snapshot()`

Set-up for R and Julia

1. `install.packages("JuliaCall")`
2. `JuliaCall::install_julia(version = "latest")`
- Installs Julia to "C:/Users/christoph.scheuch/AppData/Roaming/R/data/R/JuliaCall/julia/1.9.4/julia-1.9.4"
3. `JuliaCall::julia_setup("C:/Users/christoph.scheuch/AppData/Roaming/R/data/R/JuliaCall/julia/1.9.4/julia-1.9.4")`
3. JuliaCall::julia_setup("/Applications/Julia-1.9.app/Contents/Resources/julia/bin/") on Mac