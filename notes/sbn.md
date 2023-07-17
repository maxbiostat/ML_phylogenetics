# Computing tree probabilities from a set of trees and variational inference

- Höhna, S., & Drummond, A. J. (2012). [Guided tree topology proposals for Bayesian phylogenetic inference](https://doi.org/10.1093/sysbio/syr074). Systematic Biology, 61(1), 1-11.
  - Introduced the idea of a conditional clade probability, which assumed some independence between clades and scored trees based on the product of their CCDs.
These were then used to guide MCMC proposals.
- Larget, B. (2013). [The estimation of tree posterior probabilities using conditional clade probability distributions](https://doi.org/10.1093/sysbio/syt014). Systematic Biology, 62(4), 501-511.
  - Introduced the idea of  (approximate) **conditional independence of separated subtrees** (CISS) hypothesis.
The resulting conditional clade distributions (CCD) forgo computing the normalisation and thus are easier to compute.
- Whidden, C., & Matsen IV, F. A. (2015). [Quantifying MCMC exploration of phylogenetic tree space](https://doi.org/10.1093/sysbio/syv006). Systematic Biology, 64(3), 472-491.
  - noticed that the CCD  underestimated the posterior for sub-peaks and overestimated the posterior between peaks.
- Zhang, C., & Matsen IV, F. A. (2018). [Generalizing tree probability estimation via Bayesian networks](https://papers.nips.cc/paper_files/paper/2018/file/b137fdd1f79d56c7edf3365fea7520f2-Paper.pdf). Advances in neural information processing systems, 31.
  - Introduced the idea of subsplit Bayesian networks (SBN), which extend the CCD with a richer representation of the distribution on trees.

## Software

[bito](https://github.com/phylovi/bito) (Bayesian Inference of Trees via Optimization) is a Python/TensorFlow/PyTorch library that implements many of the SBN-related methods.

