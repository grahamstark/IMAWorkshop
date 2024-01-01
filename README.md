# IMA 2024 Julia Workshop

This is code for the 2024 IMA Conference Julia Workshop.

It would be nice if you could have a go at installing Julia ahead of the workshop as it'll save us a wee while. Installing the packages would also be good as an admitted problem with Julia is that [first time loading packages is sometimes slow](https://discourse.julialang.org/t/taking-ttfx-seriously-can-we-make-common-packages-faster-to-load-and-use/74949?page=2).

I've made a [wee video that walks you through the install steps](https://virtual-worlds.scot/imaworkshop/ima-julia-intro.mp4).

## Installing Julia

We'll be using the latest Julia 1.10, downloadable from [here](https://julialang.org/downloads/).

## Files in this repository

The files we'll be referring to are in the [src/ directory](https://github.com/grahamstark/IMAWorkshop/tree/main/src). To download them, go to the file and select the "Download Raw File" option from the icons on the top right. Alternatively, you can download everything here as a zip file by clicking on the green `Code` icon on the repository home page and selecting `Download ZIP`, or by using a Git client to clone the repository, if that's your thing.

### Installing Packages

Much of the functionality of Julia comes in packages which have to be installed separately. The file [repl-code.jl](https://github.com/grahamstark/IMAWorkshop/blob/main/src/repl-code.jl) contains code to install all the packages we'll be needing - there are packages for loading data, running regressions, plotting results and calculating inequality measures, and so on. Alteratively, just cut and paste the code below into Julia's repl. It may take a while for Julia to build everything, so this is a good thing to do before the day.

```julia 
# ==== cut and paste === 
using Pkg # Pkg is the package that manages packages.

# add some packages we'll need.
Pkg.add( "CSV" )        # delimited file reader
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
 
