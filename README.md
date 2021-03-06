# Singular

[![Build Status](https://travis-ci.org/wbhart/Singular.jl.svg?branch=master)](https://travis-ci.org/wbhart/Singular.jl)

[![Coverage Status](https://coveralls.io/repos/wbhart/Singular.jl/badge.svg?branch=master&service=github)](https://coveralls.io/github/wbhart/Singular.jl?branch=master)

[![codecov.io](http://codecov.io/github/wbhart/Singular.jl/coverage.svg?branch=master)](http://codecov.io/github/wbhart/Singular.jl?branch=master)

Julia package for using the [Singular](https://www.singular.uni-kl.de/) library for commutative and
non-commutative algebra, algebraic geometry, and singularity theory.

Currently this requires the latest Julia sources to be built, with a Make.user
file as specified in the Cxx package [README](https://github.com/Keno/Cxx.jl). Note: currently the Julia build is reported to not work with Cxx, so you might want to do git checkout 5989eaf0 in the Julia source tree before building Julia, to avoid this problem. It's a commit that is known to work with Cxx.

To build Singular.jl, start julia and then type:
```julia
julia> Pkg.add("Nemo")
julia> Pkg.checkout("Nemo")
julia> Pkg.clone("https://github.com/wbhart/Singular.jl")
julia> Pkg.build("Singular")
```
To use Singular.jl, start julia and then type:
```julia
julia> using Singular
```
