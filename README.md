# IMAWorkshop

Code for the 2024 IMA Conference Julia Workshop

## Instructions

It would be nice if you could have a go at installing Julia ahead of the workshop as it'll save us a wee while. Installing the packages would also be good as an admitted problem with Julia is that [first time loading packages is sometimes slow](https://discourse.julialang.org/t/taking-ttfx-seriously-can-we-make-common-packages-faster-to-load-and-use/74949?page=2).

### Installing Julia

We'll be using the latest Julia 1.10, downloadable from [here](https://julialang.org/downloads/).

### Files in this repository

The two files we'll be using are in the [src/ directory](https://github.com/grahamstark/IMAWorkshop/tree/main/src). You can right click over them to download them. Alternatively, you can download everything here as a zip file by clicking on the green `Code` icon on the home page and selecting '', or by using a Git client to clone the repository if that's your thing.

![Code Icon Location](https://github.com/grahamstark/IMAWorkshop/blob/main/images/ima-rep-1.png)

### Installing Packages

Much of the functionality we need comes i

```julia 
# ==== cut and paste === 

# add some packages we'll need.
Pkg.add( "CSV" )        # delimted file reader
Pkg.add( "DataFrames" ) # tables of data
Pkg.add( "Downloads" )  # allow file reading from websites
Pkg.add( "GLM" )        # linear regressions
Pkg.add( "Plots" )      # simple but powerful graphics package - Makie.jl is an alternative
Pkg.add( "Pluto" )      # Beautiful interactive workbooks
Pkg.add( "PlutoUI" )    # controls for Pluto
Pkg.add( "PovertyAndInequalityMeasures" ) # One of mine! Ginis and the like 
Pkg.add( "StatsBase" )  # means, medians ..
Pkg.add( "StatsPlots")  # specialised plots for data from dataframes

# now we have them installed, bring the packages into our code 
using CSV
using DataFrames
using Downloads
using GLM
using Plots
using Pluto
using PlutoUI
using PovertyAndInequalityMeasures
using StatsBase
using StatsPlots

# === end copy == 
```
 
