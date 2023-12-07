# [An R package `PITO`](https://github.com/hfang-bristol/PITO)

## @ Overview

> The `PITO` is an R package enabling phytomedicine (exploring evidence for genetic target prioritisation and herbal drug repurposing).

## @ Installation

### 1. Install R

Please install R (version 4.3.2 or above); see https://cran.r-project.org

If installed on `Ubuntu` (assuming you have a `ROOT (sudo)` privilege), please do so below

```ruby
sudo su
# here enter your password

wget http://www.stats.bris.ac.uk/R/src/base/R-4/R-4.3.2.tar.gz
tar xvfz R-4.3.2.tar.gz
cd ~/R-4.3.2
./configure
make
make check
make install
R # start R
```

### 2. Install R packages

```ruby
R # start R

# if the package 'BiocManager' not installed, please do so
if(!("BiocManager" %in% rownames(installed.packages()))) install.packages("BiocManager")

# first, install basic packages: remotes, tidyverse
BiocManager::install(c('remotes','tidyverse'), dependencies=T)

# then, install the package 'PITO' (now hosted at github)
BiocManager::install("hfang-bristol/PITO", dependencies=T, force=T)

# check the package 'PITO' successfully installed
library(help=PITO)
```


## @ Contact

> Please drop [email](mailto:fh12355@rjh.com.cn) for bug reports or other enquiries.


