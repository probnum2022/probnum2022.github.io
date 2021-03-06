<a href="/"><img src="gp.png" style="width: 100%; border: none; margin: -40px 0px 0px 0px; padding: none;" alt="Prob Num 2022" /></a>

<p align="center"><a href="/location">Location</a> | <a href="/participants">Participants</a> | <a href="/schedule">Schedule</a> | <a href="/talks">Talks</a></p>

# Titles and Abstracts of Talks

* [Deniz Akyıldız](#akyildiz) (Alan Turing Institute, UK, and University of Cambridge, UK)
* [Peter Challenor](#challenor) (University of Exeter, UK)
* [Philipp Hennig](#hennig) (Universität Tübingen, DE, and Max Planck Institute for Intelligent Systems, DE)
* [Toni Karvonen](#karvonen) (University of Helsinki, FI)
* [Han Cheng Lie](#lie) (Universität Potsdam, DE)
* [Maren Mahsereci](#mahsereci) (Universität Tübingen, DE)
* [Masha Naslidnyk](#naslidnyk) (University College London, UK)
* [Kamran Pentland](#pentland) (University of Warwick, UK)


<span id="akyildiz"></span>
## Deniz Akyıldız
**Alan Turing Institute, UK, and University of Cambridge, UK**

*Probabilistic sequential matrix factorization* [<a href="/pdf/akyildiz.pdf">Slides</a>]

This talk introduces a probabilistic sequential matrix factorization method for factorizing time-varying and non-stationary datasets consisting of high-dimensional time-series. In particular, we consider nonlinear Gaussian state-space models where sequential approximate inference results in the factorization of a data matrix into a dictionary and time-varying coefficients with potentially nonlinear Markovian dependencies. The assumed Markovian structure on the coefficients enables us to encode temporal dependencies into a low-dimensional feature space. The proposed inference method is solely based on an approximate extended Kalman filtering scheme, which makes the resulting method particularly efficient.


<span id="challenor"></span>
## Peter Challenor
**University of Exeter, UK**

*Inference for computer models* [<a href="/pdf/challenor.pdf">Slides</a>]

In parallel with data based modelling the use of ‘process’ based modelling has increased over recent years. This has been driven by the rise in computer power and numerical analysis techniques to allow the solution of such models. Applications abound from engineering through climate to healthcare. Although some of these models are fast to run, I will concentrate on those that are slow, meaning that any Monte Carlo based methods are implausible. To get around these problems we use surrogate models or emulators. Building such models is not trivial, involving issues in design and estimation. Once we have a validated emulator, we can address problems in inference. In particular, I will look at sensitivity and uncertainty analysis. The real inference problems occur when we want to use real world data to ‘calibrate’ the model by running it in inverse model. The problem here is the problem of model ‘discrepancy’. Because the model is a model it is never going to be the same as the real world and we need to take this into account. I’ll outline a couple of ways of doing this: the Kennedy and O’Hagan method and History Matching. Finally, I will point out some open research questions.


<span id="hennig"></span>
## Philipp Hennig
**Universität Tübingen, DE, and Max Planck Institute for Intelligent Systems, DE**

*Backward and Inverse: Opportunities for Probnum in Machine Learning* [<a href="/pdf/hennig.pdf">Slides</a>]

Aiming to advertise killer applications for probabilistic numerics, I will highlight two separate areas: First, in inverse problems involving simulations, ODE filters have shown (occasionally drastic) efficiency gains over classical methods by leveraging uncertainty propagation through computation. 

Secondly, deep learning continues to pose formidable algorithmic challenges for its users. I will argue that probnum has the potential to contribute significantly here, because the relevant computations are inherently probabilistic. It used to be difficult to capitalise on this opportunity. But recently released software libraries now provide access to detailed statistics, providing a new playing field to the probnum community. 


<span id="karvonen"></span>
## Toni Karvonen
**University of Helsinki, FI**

*Why not to use the Gaussian kernel* [<a href="/pdf/karvonen.pdf">Slides</a>]

In Gaussian process modelling it is common to use the Gaussian (or squared exponential) kernel as the default covariance kernel. In this talk I use numerical ill-conditioning, analyticity and super-exponential rates of convergence in the RKHS to argue that the Gaussian kernel is not robust and should not be used in Bayesian quadrature and other the interpolatory settings where the data are assumed noiseless.


<span id="lie"></span>
## Han Cheng Lie
**Universität Potsdam, DE**

*Randomised time integration of operator differential equations*

The paper of Conrad et al. (*Statistics and Computing*, 2017) played an important role in establishing the idea of putting probability measures on numerical solutions of differential equations on finite-dimensional Euclidean space. We revisit some ideas from this paper, for differential equations on Banach spaces of arbitrary and possibly infinite dimension, and for time integration methods on possibly nonuniform grids. First, we present an analytical example involving a heat equation on a bounded domain, in which one can 'read off' the effect of randomisation on the Bayesian posterior on the parameter space. Second, we show that, by using a different error decomposition, one can weaken the assumption of uniform local truncation error on the underlying deterministic time integration method. This significantly improves the applicability of randomised time integration methods. If time permits, we will discuss to what extent the bounds on the mean squared error of the randomised solutions presented by Conrad et al. extend to errors of higher integrability order.

Joint work with Martin Stahn (U. Potsdam) and T. J. Sullivan (U. Warwick).


<span id="mahsereci"></span>
## Maren Mahsereci
**Universität Tübingen, DE**

*ProbNum: Probabilistic Numerics in Python* [<a href="/pdf/mahsereci.pdf">Slides</a>]

Providing quality code increases trust in methods and has become an integral part of research these days. As a small field, probabilistic numerics can benefit from such a platform. The talk motivates ProbNum, a Python library that provides probabilistic numerical solvers for differential equations, linear systems, and integration problems. It is hosted on GitHub and maintained by several members of the community. The talk highlights how users can get in touch with probabilistic numerics via ProbNum and the tutorials provided. Further, PN researchers may benefit from ProbNum as well as new projects can be build fast and robustly using existing, well-tested components. This is illustrated with some functional examples.


<span id="naslidnyk"></span>
## Masha Naslidnyk
**University College London, UK**

*On robust GP regression* [<a href="/pdf/naslidnyk.pdf">Slides</a>]

Kernel selection for Gaussian process regression has a defining effect on the quality of the model. Maximum likelihood estimation, the most popular approach for selecting a kernel from a parametrised family, has been shown empirically to perform worse under model misspecification compared to cross-validation; theoretical analysis has been missing. In this work, we provide theoretical and empirical evidence that, for noiseless one-dimensional Gaussian process regression with a Brownian motion kernel, cross-validation estimator is more robust to undersmoothing (meaning an insufficiently smooth kernel) than maximum likelihood estimator. Finally, I'll discuss a recent research direction on using maximum mean discrepancy for general parameter selection in conditional models.


<span id="pentland"></span>
## Kamran Pentland
**University of Warwick, UK**

*GParareal: a time-parallel ODE solver using Gaussian process emulation* [<a href="/pdf/pentland.pdf">Slides</a>]

Sequential numerical methods for integrating initial value problems (IVPs) can be prohibitively expensive when high numerical accuracy is required over the entire interval of integration. One remedy is to integrate in a parallel fashion, "predicting" the solution serially using a cheap (coarse) solver and "correcting" these values using an expensive (fine) solver that runs in parallel on a number of temporal subintervals. In this work, we propose a time-parallel algorithm (GParareal) that solves IVPs by modelling the correction term, i.e. the difference between fine and coarse solutions, using a Gaussian process emulator. This approach compares favourably with the classic parareal algorithm and we demonstrate, on a number of IVPs, that GParareal can converge in fewer iterations than parareal, leading to an increase in parallel speed-up. GParareal also manages to locate solutions to certain IVPs where parareal fails and has the additional advantage of being able to use archives of legacy solutions, e.g. solutions from prior runs of the IVP for different initial conditions, to further accelerate convergence of the method - something that existing time-parallel methods do not do.
