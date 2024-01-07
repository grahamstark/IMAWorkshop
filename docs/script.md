# script


Hi 

I have 1 1/2 hours to persuade you of why you should use Julia

I circulated a note - 

if you haven't seen it it's here: https://github.com/grahamstark/IMAWorkshop/

There's material there you can cut and paste.


Pitch: Julia is fun, gets results quickly (with one caveat), solves 2 language problem - no estimating in Stata, model building in Fortran.

So, lets start with some examples (these are running on quite a tempremental web server):


https://stb.virtual-worlds.scot/bcd/ Messy relationship between earnings and net income
https://triplepc.northumbria.ac.uk/  Fiscal changes and popularity 

but for *really* interesting stuff, try:

https://computationalthinking.mit.edu/Fall23/ MIT Computational Thinking Course

If you haven't installed, let's try now. Choose local if locked down.

I know about tax benefit models, so that's what I've chosen to introduce this with. I'm going to walk you through building a simple model. If we have time, we can then look at a fancier model, or experiment with Julia's excellent data science facilties.

There are thousands of packages. Important things we won't have time for include optimising, agent based models, Makie (a newer and fancier graphics)..

So lets start. We'll import one package: Pluto. It's just a nice web-based notebook system.

[mess around for 5]

url="https://virtual-worlds.scot/ou/uk-lcf-subset-2005-6.csv"
lcf = Downloads.download(url) |> CSV.File |> DataFrame 


