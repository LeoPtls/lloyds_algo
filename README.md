## Lloyd’s algorithms for optimal and uniform quantization

This small project is devoted to a graphical representation of the
iterates of Lloyd’s algorithms for both optimal and uniform quantization
of measures. 
That is, the algorithm solves

$$
\underset{(Y,\pi)\in (\mathbb{R}^{d})^N\times \Delta_N}{\min} \qquad W\_{2}^{2}\left(\mu,\sum\_{i=1}^{N}\pi_i \delta\_{y\_{i}}\right)
$$

and

$$
\underset{Y\in (\mathbb{R}^{d})^N}{\min} \qquad W\_{2}^{2}\left(\mu,\frac{1}{N}\sum\_{i=1}^{N} \delta\_{y\_{i}}\right)
$$

where *μ* is a (continuous) target measure. [Lloyd’s
algorithm](https://en.wikipedia.org/wiki/Lloyd%27s_algorithm) (which
solves the K-means problem) is a fixed point iteration that alternates
between the computation of a partition of a set of points (Voronoï or
Laguerre) and the update of those points to the centroids of the sets of
this partition. We studied the sequential convergence (that is, to a
single point cloud) of these iterates[^1]. Using the
[PyMongeAmpere](https://github.com/mrgt/PyMongeAmpere) library made by
Quentin Mérigot we illustrates this result empirically. The target
measure we consider is a mixture of two Gaussians.

[^1]: L Portales, E Cazelles, E Pauwels. On the sequential convergence
    of Lloyd’s algorithms. 2025
