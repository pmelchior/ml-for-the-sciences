Mixture model applications
==========================

Mixture models are a very general and useful tool. Here are a few scientific papers that utilize mixture models in a variety of contexts from Bayesian inference to distribution function modeling of stellar orbits.

Data-driven models:
- [**Bovy et al. 2010**](https://arxiv.org/abs/1011.6392)

  They use extreme deconvolution (XD) to build a star/quasar classifier to be
  used for spectroscopic target selection for the SDSS.

- [**Anderson et al. 2017**](https://arxiv.org/abs/1706.05055)

  We used XD to infer the density of sources in the color-magnitude diagram,
  then used the inferred density to improve distance estimates for faint/distant
  stars in Gaia DR1.

- [**Melchior & Goulding 2016**](https://arxiv.org/abs/1611.05806)

  This is the paper describing the method Peter spoke about a few weeks ago: XD
  with support for incomplete data. They apply it to the problem of deconvolving
  an X-ray (Chandra) image of a nearby galaxy that has masked regions, chip
  gaps, and known sensitivity variations across the detector.

Mixture-models in likelihoods:
- [**Hogg et al. 2010**](https://arxiv.org/abs/1008.4686)

  Section 3 describes how to fit a model in the presence of outliers in a
  probabilistic sense. The likelihood simplifies to being a mixture model. See
  also [Dan F-M's blog post](http://dfm.io/posts/mixture-models/).

- [**Price-Whelan et al. 2015**](https://arxiv.org/abs/1503.08780)

  This is just an example application of the outlier model from Hogg et al.
  2010.

Mixture-models for convenience:
- [**Oh et al. 2017**](https://arxiv.org/abs/1612.02440)

  Used a Gaussian mixture model to represent the true distribution of velocities in the Milky Way disk, i.e. as a prior. In principle, we could have used any distribution with tails, but using a GMM with a Gaussian likelihood meant that many marginalizations are analytic.
  
- [**Hogg & Lang 2012**](http://cosmo.nyu.edu/hogg/research/2012/10/23/mixture_models.pdf) and [**Sheldon 2014**](https://arxiv.org/abs/1403.7669)
  
  Replace the Sersic model for galaxies with a mixture of Gaussians, so that convolution with the PSF (also represented as mixture of Gaussian) becomes analytic and fast.

- Also ask Scott Carlsten about his project!

Flexible theoretical models:

- [**Magorrian 2013**](https://arxiv.org/abs/1303.6099)
