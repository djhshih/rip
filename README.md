# rip

rip is a command line installer for R packages.

## Installation

You'll have to install the `argparser` R package using the traditional method in
R:

```r
install.packages("argparser")
```

Then, simply place `rip` in a directory included in the `$PATH` environmental
variable, such as `/usr/bin`.


## Usage

The main advantage of using `rip` is that it can simply installation of a set of
dependencies. Suppose you have a file named `requirements.txt` as follows:

```
io
ggplot2
magrittr
dplyr
tidyr
```

Then within this directory, you can simply install all the packages by

```bash
rip install
```

For more information, call `rip` without any arguments.

