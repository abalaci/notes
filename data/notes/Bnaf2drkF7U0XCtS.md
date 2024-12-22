
## Notes

- Most popular technique for estimating probability densities of random variables
- A chosen kernel function is applied for each point in the finite dataset
- Many possible kernel functions, such as, but not limited to:
  - Gaussian (normal)
  - Triangular
  - Rectangular (uniform/box)
  - Epanechnikov (parabolic)
  - Biweight (quartic)
  - Triweight
  - Tricube
  - Cosine
- One can choose different kernel widths
- Adaptive KDE

## Formula

$$
f(x) = \frac{1}{nh}\sum_{i=1}^{n}K(\frac{x-x_i}{h})
$$

where $n$ is the number of sample, $h$ is the *bandwidth* and $K$ is the *kernel function*.

## References

- https://en.wikipedia.org/wiki/Kernel_density_estimation
- https://en.wikipedia.org/wiki/Kernel_(statistics)#Kernel_functions_in_common_use
- http://www.mit.edu/~talw/publications/kde_space_full.pdf
- https://towardsdatascience.com/modality-tests-and-kernel-density-estimations-3f349bb9e595
- https://bmcproc.biomedcentral.com/articles/10.1186/1753-6561-7-S7-S7
- http://faculty.washington.edu/yenchic/18W_425/Lec6_hist_KDE.pdf
- https://stats.stackexchange.com/questions/219833/density-estimation-for-large-dataset

## Implementations

- https://cran.r-project.org/web/packages/kedd/vignettes/kedd.pdf
- https://stat.ethz.ch/R-manual/R-devel/library/stats/html/density.html
- https://stat.ethz.ch/R-manual/R-devel/library/KernSmooth/html/bkde.html
- https://jakevdp.github.io/PythonDataScienceHandbook/05.13-kernel-density-estimation.html

## Articles & Papers

- https://aakinshin.net/posts/kde-bw/
- https://aakinshin.net/posts/discrete-sample-jittering/
- https://www.cs.utah.edu/~lifeifei/papers/kernelsigmod13.pdf
- http://www.econ.upf.edu/~lugosi/l1testrev.pdf
