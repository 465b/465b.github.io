# Overview of present marine ecosystem modelling Frameworks

Developing new ecosystem models is generally done through two approaches. Either the model is written from scratch or a modelling framework is used. While writing a a new model from scratch offers the most flexibility it is also the most time consuming. Frameworks, assist in that process by offering parts of the functionality that is necessary for all applications in that context.

However, because there exist several different typical modelling approaches there also different frameworks which work for a certain subset of model types. We present a list of the currently present marine ecosystem model frameworks, to assist in the choice of a suitable one.

## Forward Modelling Frameworks

### QPress

QPress is a R package for qualitative network modelling. It implements a simulation approach to sample many iterations of the community interaction matrix that corresponds with a specified signed digraph. This means that, for each link, simulations sample across the range of possible strengths. Uncertain links are down-weighted by randomised exclusion from simulations. Only those iterations that are stable are maintained, and the responses are aggregated to provide a probabilistic interpretation of qualitative outcomes, i.e. the probability of a long-term population increase or decrease for each group in the model under a given press perturbation scenario.

[Related publication](https://doi.org/10.1016/j.marpol.2020.103832)

[QPress on GitHub](https://github.com/SWotherspoon/QPress)

## Inverse Modelling Frameworks

### AD Model builder

Many criteria for statistical parameter estimation, such as maximum likelihood, are formulated as a nonlinear optimization problem.Automatic Differentiation Model Builder \(ADMB\) is a programming framework based on automatic differentiation, aimed at highly nonlinear models with a large number of parameters. The benefits of using AD are computational efficiency and high numerical accuracy, both crucial in many practical problems. We describe the basic components and the underlying philosophy of ADMB, with an emphasis on functionality found in no other statistical software. One example of such a feature is the generic implementation of Laplace approximation of high-dimensional integrals for use in latent variable models. We also review the literature in which ADMB has been used, and discuss future development of ADMB as an open source project. Overall, the main advantages of ADMB are flexibility, speed, precision, stability and built-in methods to quantify uncertainty.

[Related Publication](https://www.tandfonline.com/doi/full/10.1080/10556788.2011.597854)

[Official Website](http://www.admb-project.org/)

### Calibrar

Automated parameter estimation for complex \(ecological\) models in R. This package allows the parameter estimation or calibration of complex models,including stochastic ones. It is a generic tool that can be used for fitting any type of models, especially those with non-differentiable objective functions.It supports multiple phases and constrained optimization.It implements maximum likelihood estimation methods and automated construction of the objective function from simulated model outputs.

[Calibrar on GitHub](http://roliveros-ramos.github.io/calibrar)

[Package Documentation](https://cran.r-project.org/web/packages/calibrar/calibrar.pdf)

## Forward and inverse modelling Frameworks

### GADGET

Gadget is the Globally applicable Area-Disaggregated General EcosystemToolbox. Gadget is a powerful and flexible framework that has been developed to model complicated statistical marine ecosystems within a fish-eries management and biological context, and can take many features of the ecosystem into account. Gadget allows the user to include a number of features of the ecosystem into the model: One or more species, each ofwhich may be split into multiple components; multiple areas with migration between areas; predation between and within species; growth; maturation; reproduction and recruitment; multiple commercial and survey fleets taking catches from the populations. Gadget works by running aninternal forward projection model based on many parameters describingthe ecosystem, and then comparing the output from this model to ob-served measurements to get a likelihood score. The model ecosystem pa-rameters can then be adjusted, and the model re-run, until an optimum isfound, which corresponds to the model with the lowest likelihood score.This iterative, computationally intensive process is handled within Gad-get, using a robust minimisation algorithm. Gadget has successfully beenused to investigate the population dynamics of stock complexes in Ice-landic waters, the Barents Sea, the North Sea, the Irish and Celtic Seas andthe Sofala Bank fishery of Mozambique. This paper describes the structureand main components of an ecosystem model developed using the Gadgetframework.

[Gadget self-publication](https://core.ac.uk/reader/52043609)

[Gadget on GitHub](https://github.com/Hafro/gadget2)

### FABM + ParSAC

One of the most of challenging steps in the development of coupled hydrodynamic-biogeochemical models is the combination of multiple, often incompatible computer codes that describe individual physical, chemical, biological and geological processes. This “coupling” is time-consuming, error-prone, and demanding in terms of scientific and programming expertise. The open source, Fortran-based Framework for Aquatic Biogeochemical Models addresses these problems by providing a consistent set of programming interfaces through which hydrodynamic and biogeochemical models communicate. Models are coded once to connect to FABM, after which arbitrary combinations of hydrodynamic and biogeochemical models can be made. Thus, a biogeochemical model code works unmodified within models of a chemostat, a vertically structured water column, and a three-dimensional basin. Moreover, complex biogeochemistry can be distributed over many compact, self-contained modules, coupled at run-time. By enabling distributed development and user-controlled coupling of biogeochemical models, FABM enables optimal use of the expertise of scientists, programmers and end-users.

[Publication](https://doi.org/10.1016/j.envsoft.2014.04.002)

[FABM on GitHub](https://github.com/fabm-model/fabm)

### Ecopath \(with Ecoism\)

The Ecopath with Ecosim \(EwE\) modeling approach combines software for ecosystem trophic mass balance analysis \(Ecopath\), with a dynamic modeling capability \(Ecosim\) for exploring past and future impacts of fishing and environmental disturbances as well as for exploring optimal fishing policies. Ecosim models can be replicated over a spatial map grid \(Ecospace\) to allow exploration of policies such as marine protected areas, while accounting for spatial dispersal/advection effects. The Ecopath approach and software has been under development for two decades, with Ecosim emerging in 1995, and Ecospace in 1998, leading to an integrated and widely applied package. We present an overview of the computational aspects of the Ecopath, Ecosim and Ecospace modules as they are implemented in the most recent software version.

[Publication](http://doi.org/10.1016/j.ecolmodel.2003.09.003)

### Atlantis

Atlantis was developed at CSIRO \(Australia\) as an ‘end-to-end’ simulation modeling approach for marine ecosystems that includes oceanographic, chemical \(nutrient cycling\), ecological \(competition and predation\), and anthropogenic processes in a three-dimensional, spatially explicit domain. Atlantis is intended as a strategic management tool to evaluate hypotheses about ecosystem response, to understand cumulative impacts of human activities, and to rank broad categories of management options.

[Webpage](https://www.nwfsc.noaa.gov/research/divisions/cb/ecosystem/marineecology/aem.cfm)

[User Guide](https://research.csiro.au/atlantis/?ddownload=111)

