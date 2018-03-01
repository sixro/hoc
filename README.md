# hoc

Hits-of-Code. For details about this script, check [this article](http://www.yegor256.com/2014/11/14/hits-of-code.html) by Yegor Bugayenko.

The script requires that you have installed on your system the following softwares:

  * git
  * grep 
  * awk 


## Installation

This is a shell script (`/bin/sh`). So you have simply to clone this project and probably put it in your `PATH`.


## Usage

```
Usage: hoc [OPTIONS]... [PRJDIR]
where OPTIONS can be:
	-v       enable verbose output (default: false)
	-s       set the date since you need hoc (default: today)
	-t       set the date till you need hoc (default: today)
	-f       set a filter on all files to calculate an hoc on specific files/dirs (default: none)
and PRJDIR represents the (parent) project maven dir (default: current dir)

Software required: git, grep and awk
```


## an example

Pressing the following command in the same local working copy of this repo:

```
hoc -s 2018-01-01 .
```

you should obtains something like:

```
10 Roberto Simoni
```

where the 1st number is the `hoc` for the git user `Roberto Simoni`.  
With that you can manipulate data with other shell softwares.
The filter option (`-f`) could be useful to analyze specific directories, modules, files, etc...
