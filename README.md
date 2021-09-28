# rip

`rip` is a command line installer for R packages.

## Installation

Download a release archive, extract it, and place `rip` in a 
directory included in the `$PATH` environmental variable, such as `/usr/local/bin`.

If you are on Linux, you can also do

```bash
curl -L https://github.com/djhshih/rip/archive/v0.4.tar.gz | \
	tar -xz --strip-components=1 rip-*/rip
install rip /usr/local/bin && rm rip
```

Note that the second line requires root permission (`sudo`).


## Usage

The main advantage of using `rip` is that it facilitates installation of 
multiple dependencies. Suppose you are in a directory with a file named 
`requirements.txt` containing:

```
io
magrittr
ggplot2
dplyr
tidyr
stringr
lubridate
devtools
roxygen2
testthat
```

Then you can simply install all above packages by

```bash
rip install
```

For more information, call `rip` without any arguments.

