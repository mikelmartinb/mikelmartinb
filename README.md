# Mikel Martin Barandiaran

PhD student in theoretical cosmology at the [Instituto de Física Teórica (IFT UAM-CSIC)](https://www.ift.uam-csic.es), Madrid.

I work on cosmic topology and tests of statistical isotropy, large-scale structure, the cosmic microwave background and higher-order statistics, on both the theory and the numerical side. I am a core member of the [COMPACT Collaboration](https://github.com/CompactCollaboration), and in the Euclid Collaboration I lead the team working on the cosmic-dipole measurement (Theory Working Group).

[Website](https://sites.google.com/view/mikelmartinb/home) · [INSPIRE-HEP](https://inspirehep.net/authors/2703526) · [ORCID](https://orcid.org/0009-0004-8247-9584) · [mikel.martin@uam.es](mailto:mikel.martin@uam.es)

## Code

### [CMB-for-S3](https://github.com/CompactCollaboration/CMB-for-S3) · COMPACT Collaboration

CMB correlation matrices for a closed universe with the topology of the three-sphere or of a lens space. When space is multiply connected, statistical isotropy is broken: the harmonic-space covariance matrix is no longer diagonal and depends on where the observer sits. Python and Cython, with an example notebook and a script for computing many matrices on a cluster.

- **Paper:** *Cosmic topology. Part IId. Eigenmodes and correlation matrices of lens spaces*, Martin Barandiaran et al., COMPACT Collaboration (2026), [arXiv:2610.12418](https://arxiv.org/abs/2610.12418).

<!-- CHECK: is wigner_d_jacobi.pyx in this repo the Wigner-d code you plan to release separately? If so, the RS line "will be public by [date]" can say it is already public here. -->

### [fast_wigner_d](https://github.com/mikelmartinb/fast_wigner_d)

Wigner d- and D-matrices for integer and half-integer spin at any angle, as a small Cython extension with optional OpenMP parallelisation. Half-integer spins are what you need for eigenmodes on the three-sphere, and common recursion-based libraries do not support them. Matrix elements are computed from Jacobi polynomials in log space to avoid overflow, with absolute errors of about 10⁻¹⁴ up to j = 2000 when checked against mpmath. The repository includes tests, an example notebook and benchmarks against spherical, wigner, SciPy and sympy. 

### [MorphoMarks](https://github.com/mikelmartinb/MorphoMarks)

Marked power spectra in which the density field is weighted by its local morphology: tidal shear, isotropy, filamentarity and a fractal-dimension estimator. Includes the tools to build the density field and the tidal-tensor eigenvalues, and an example notebook.

- **Paper:** *Weighted Webs: Morphology-Informed Marked Fields*, Martin Barandiaran, Cowell, Alonso, Carrón Duque & García-Bellido (2026), [arXiv:2607.26021](https://arxiv.org/abs/2607.26021).

### [MFs4HPA](https://github.com/mikelmartinb/MFs4HPA)

Minkowski functionals on local patches of the *Planck* CMB map, to test whether the hemispherical power asymmetry also shows up in the morphology of the fluctuations and not only in their variance. The functionals are computed with [Pynkowski](https://github.com/javicarron/pynkowski) (designed for a cluster), and the analysis notebook reproduces the results of the paper.

- **Paper:** *More Than Power: Revisiting the CMB Hemispherical Power Asymmetry with Morphological Descriptors*, Carrón Duque, Martin Barandiaran & Martínez-Arrizabalaga (2026), [arXiv:2603.22449](https://arxiv.org/abs/2603.22449).

<!-- Add the standalone Wigner-d library here once it is released. -->
