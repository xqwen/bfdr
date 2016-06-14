# R code for Bayesian FDR control

This repository contains R code to perfrom Robust Bayesian FDR control. The statistical methods are described in this [manuscript](https://arxiv.org/abs/1311.3981). 


## License

Software distributed under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. See [LICENSE](http://www.gnu.org/licenses/gpl-3.0.en.html) for more details.


## R functions

* ``EBF_fdr`` implements the EBF procedure, which estimates upper-bound of pi_0 using sample mean. The input to the function consists of a vector of pre-computed Bayes factors and the alpha-level for FDR control (if ignored, alpha is set to 0.05)


* ``BF_fdr`` implements a generic Bayes factor-based Bayesian FDR control procedure. Comparing to the ``EBF_fdr`` fucntion, it requires an additional parameter pi_0 to be specified. Typically, this function is used when pi_0 is estimated based on sample quantiles (i.e., the QBF procedure).


 
## Reference and Citation

Wen, X. Robust Bayesian FDR Control using Bayes Factors, with Applications to Multi-tissue eQTL Discovery. Statistics in Biosciences (In press).
