# Deep Learning for Quadratic Hedging in Incomplete Jump Market

This is a code repository fot the deep learning algorith described in the paper [Deep Learning for Quadratic Hedging in Incomplete Jump Market](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4371396) writen by Dr. Nacira Agram, Dr. Bernt Øksendal and Jan Rems. Algorithm is implemented for cases of continous and jump financial markets.

## Code File List:
- **DeepSolver.py**: This file contains the deep learning algorithm introduced in our paper. Additionaly solver and evaluator classes are defined.
- **DataGenerator.py**: Here random inputs for construction of SDEs are generated for different type of SDEs.
- **Plots.py**: This file is used to generate and store graphic results of the simulations

The following files are used for implementation of different type of financial models:
- **BlackScholesModel.py**: Implementation of the Black Scholes model. Comparison with analytical solutions is available. Generalized for multi-dimensional Brownian motion case.
- **MertonModel.py**: Implementation of the Merton model. Initial value estimation for benchmark solutions is available through Monte Carlo simulations. Generalized for multi-dimensional Brownian motion and jump process case.
- **MixedMertonModel.py**: Implementation of one-dimensional Merton model where jumps come from mixed distributions. Allows results comparison for multi-dimensional Merton model.
- **DoubleExponential.py**: Implementation of the Kou's double exponential jump diffusion model. Initial value Monte Carlo estimation is not stable for some choices of parameters.

## Instructions on running code:

Deepending on the financial model of choice one must set desired parameters at the top of the corresponding model file and run it. Code will automatically create directories where it will store the network weights and the graphs.

