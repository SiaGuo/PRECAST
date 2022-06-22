# PRECAST
PRECAST: a probabilistic embedding and clustering with alignment for spatial transcriptomics data integration.

# Installation

To install the the packages `PRECAST`, firstly, install the `remotes` package. Besides, `PRECAST` depends on the  `scater` R package on Bioconductor. Users require to install the `BiocManager`, then use the command below to install these two packages.

In addtion, "PRECAST" depends on the 'Rcpp' and 'RcppArmadillo' package, which also requires appropriate setting of Rtools and Xcode for Windows and Mac OS/X, respectively.
```{Rmd}
# install BiocManager
install.packages("BiocManager")
# install the package on Bioconducter
BiocManager::install(c("scater"))

# Install PRECAST from github
install.packages("remotes")
remotes::install_github("feiyoung/PRECAST")
```



# Setup on Windows system
First, download [Rtools](https://cran.r-project.org/bin/windows/Rtools/); second, add the Rtools directory to the environment variable. Users can follow [here](https://helpdeskgeek.com/windows-10/add-windows-path-environment-variable/#:~:text=Go%20ahead%20and%20click%20on%20the%20Environment%20Variables,you%20have%20to%20decide%20which%20one%20to%20edit) to add Windows PATH Environment Variable.


# Setup on MacOS system
Installation about Xcode can be referred [here](https://stackoverflow.com/questions/8291146/xcode-installation-on-mac#:~:text=You%20get%20it%20from%20the%20Mac%20App%20Store.,find%20the%20app%2C%20and%20click%20the%20install%20button).

# Setup on Linux  system
If you use conda environment on Linux system and some dependent packages (such as `scater`) can not normally installed, you can search R package at [here](https://anaconda.org/). We take the `scater` package as example, and its search result is [here](https://anaconda.org/bioconda/bioconductor-scater). Then you can install it in conda environment by following command.
```{Linux}

conda install -c bioconda bioconductor-scater
```

For running big data, users can use the following system command to set the C_stack unlimited in case of `R Error: C stack usage is too close to the limit`.
```{Linux}
ulimit -s unlimited
```

# Demonstration

For an example of typical PRECAST usage, please see our [Package Website](https://feiyoung.github.io/PRECAST/index.html) for a demonstration and overview of the functions included in PRECAST.