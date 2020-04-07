# Risk Trading in a Chance-Constrained Stochastic Electricity Market
Repository containing supplementary data and code for the paper "*Risk Trading in a Chance-Constrained Stochastic Electricity Market*" by Robert Mieth, Matt Roveto and Yury Dvorkin.
If you use this code or its for academic purposes please cite this paper. 

**Instructions:**

The optimization model was implemented by using [JuMP](https://github.com/JuliaOpt/JuMP.jl) and auxiliary packages in the [Julia](http://julialang.org/downloads/) programming language.
Additionally, we used Mosek 8.1.0.63 in our numerical experiments. [Mosek](https://www.mosek.com) is a commercial solver which must be installed and licensed (e.g. using an academic license). The solver was chosen for its specific features for second-order conic programming. For more information on solvers, see the JuMP documentation.

The experiments require Julia 1.3. All necessary packages and their respective versions are distributed in the `Project.toml` file. The packages can be loaded in a new Julia environment directly via the Julia package manager IDE or running: 
```
julia> import Pkg
julia> Pkg.activate(".")
julia> Pkg.instantiate()
```

**Running the code:**

An exemplary case study with all model formulations provided as a Jupyter Notebook `risk_trading_case_study.ipynb`.
To run the notebook install the `IJulia` package:
```
julia> Pkg.add("IJulia")
```
and then in your terminal:
```
jupyter notebook risk_trading_case_study.ipynb
```
