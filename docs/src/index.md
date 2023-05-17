```@raw html
<script async defer src="https://buttons.github.io/buttons.js"></script>
<span style="color: #9558B2;font-size:4.5em;">
StatisticalMeasures.jl</span>
<br>
<span style="color: #9558B2;font-size:1.6em;font-style:italic;">
Measures (metrics) for statistics and machine learning</span>
<br><br>
```

### Quick links

- [Index of measures and their aliases](@ref aliases)
- [Examples of Usage](@ref)


# Overview

This package defines common measures (metrics) for classification and regression problems
in statistics and machine learning. To see if your favorite measures is implemented, see
[this list](@ref aliases). Some multi-target measures are included, but see also [Custom
multi-target measures](@ref).

Measures with parameters (e.g., the ``L^p`` loss) are realized as callable instances of a
struct; [calling syntax](@ref calling) complies with the specification in
[StatisticalMeasuresBase.jl](https://github.com/JuliaAI/StatisticalMeasuresBase.jl).


In addition to the measures themselves, this package provides:

- A tool [`roc_curve`](@ref) for plotting Receiver Operator Characteristics

- An extension module allowing measures from
  [LossFunctions.jl](https://github.com/JuliaML/LossFunctions.jl) to be used and extended
  using the same syntax as other measures. See [Using losses from LossFunctions.jl](@ref).

- A submodule `ConfusionMatrices` providing a confusion matrix type and basic
  functionality.

- A submodule `Functions` where some core measure implementations are factored out as
  pure functions.
  