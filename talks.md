<a href="/"><img src="gp.png" style="width: 100%; border: none; padding: none;" alt="Prob Num 2022" /></a>

<p align="center"><a href="/location">Location</a> | <a href="/participants">Participants</a> | <a href="/schedule">Schedule</a> | <a href="/talks">Talks</a></p>

# Titles and Abstracts of Talks

* [Deniz Akyıldız](#akyildiz) (Alan Turing Institute, UK, and University of Cambridge, UK)
* [Philipp Hennig](#hennig) (Universität Tübingen, DE)
* [Toni Karvonen](#karvonen) (University of Helsinki, FI)
* [Kamran Pentland](#pentland) (University of Warwick, UK)


<span id="akyildiz"></span>
## Deniz Akyıldız
**Alan Turing Institute, UK, and University of Cambridge, UK**

*Probabilistic sequential matrix factorization*

This talk introduces a probabilistic sequential matrix factorization method for factorizing time-varying and non-stationary datasets consisting of high-dimensional time-series. In particular, we consider nonlinear Gaussian state-space models where sequential approximate inference results in the factorization of a data matrix into a dictionary and time-varying coefficients with potentially nonlinear Markovian dependencies. The assumed Markovian structure on the coefficients enables us to encode temporal dependencies into a low-dimensional feature space. The proposed inference method is solely based on an approximate extended Kalman filtering scheme, which makes the resulting method particularly efficient. 


<span id="hennig"></span>
## Philipp Hennig
**Universität Tübingen, DE**

*Backward and Inverse: Opportunities for Probnum in Machine Learning*

Aiming to advertise killer applications for probabilistic numerics, I will highlight two separate areas: First, in inverse problems involving simulations, ODE filters have shown (occasionally drastic) efficiency gains over classical methods by leveraging uncertainty propagation through computation. 

Secondly, deep learning continues to pose formidable algorithmic challenges for its users. I will argue that probnum has the potential to contribute significantly here, because the relevant computations are inherently probabilistic. It used to be difficult to capitalise on this opportunity. But recently released software libraries now provide access to detailed statistics, providing a new playing field to the probnum community. 


<span id="karvonen"></span>
## Toni Karvonen
**University of Helsinki, FI**

*Why not to use the Gaussian kernel*

In Gaussian process modelling it is common to use the Gaussian (or squared exponential) kernel as the default covariance kernel. In this talk I use numerical ill-conditioning, analyticity and super-exponential rates of convergence in the RKHS to argue that the Gaussian kernel is not robust and should not be used in Bayesian quadrature and other the interpolatory settings where the data are assumed noiseless.


<span id="pentland"></span>
## Kamran Pentland
**University of Warwick, UK**

*GParareal: a time-parallel ODE solver using Gaussian process emulation*

Sequential numerical methods for integrating initial value problems (IVPs) can be prohibitively expensive when high numerical accuracy is required over the entire interval of integration. One remedy is to integrate in a parallel fashion, "predicting" the solution serially using a cheap (coarse) solver and "correcting" these values using an expensive (fine) solver that runs in parallel on a number of temporal subintervals. In this work, we propose a time-parallel algorithm (GParareal) that solves IVPs by modelling the correction term, i.e. the difference between fine and coarse solutions, using a Gaussian process emulator. This approach compares favourably with the classic parareal algorithm and we demonstrate, on a number of IVPs, that GParareal can converge in fewer iterations than parareal, leading to an increase in parallel speed-up. GParareal also manages to locate solutions to certain IVPs where parareal fails and has the additional advantage of being able to use archives of legacy solutions, e.g. solutions from prior runs of the IVP for different initial conditions, to further accelerate convergence of the method - something that existing time-parallel methods do not do.
