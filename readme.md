# Bayes Project Notes

## General Theory

Statistical Rethinking - Richard McElreath. 2nd Edition coming out Spring 2020. Lectures that follow book are on [YouTube](https://www.youtube.com/watch?v=4WVelCswXo4&list=PLDcUM9US4XdNM4Edgs7weiyIguLSToZRI). Really readable.

[Bayesian Data Analysis](https://www.amazon.co.uk/Bayesian-Analysis-Chapman-Statistical-Science/dp/1439840954) - Andrew Gelman's book, considered the bible of Bayesian data analysis (haven't read it). Also see [Andrew's blog](https://statmodeling.stat.columbia.edu/)

[Doing Bayesian Analysis](https://www.amazon.co.uk/Doing-Bayesian-Data-Analysis-Tutorial-ebook/dp/B00PYZ2VR6/ref=dp_kinw_strp_1) - John Kruschke

[Bayesian Methods for Hackers](http://camdavidsonpilon.github.io/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/) - Cam DavidsonPilon. Good mix of code and theory. Good to see the numpy and matplotlib code.

[Michael Betancourt](https://betanalpha.github.io/) - very prominant Bayesian statistician, writes case studies covering bayes mcmc theory and applications.

## Applications in P&C/GI
- [Loss development curves in Stan - Mick Cooney](https://github.com/InsuranceDataScience/StanWorkshop2018/tree/master/loss_curves)
- [Hierarchical compartmental reserving models - Jake Morris](hhttps://github.com/InsuranceDataScience/StanWorkshop2018/master/loss_curves/compart_models.html#/)
- [Loss Curves - Mick Cooney, 2017](https://github.com/kaybenleroll/stancasestudy_losscurves)
- [Hierarchical loss reserving with growth cruves using brms - Markus Gesmann](https://magesblog.com/post/2018-07-15-hierarchical-loss-reserving-with-growth-cruves-using-brms/)
- [Hierarchical loss reserving with stan - Markus Gesmann](https://magesblog.com/post/2015-11-10-hierarchical-loss-reserving-with-stan/)
- [Loss Developments via Growth Curves and Stan - Markus Gesmann](https://magesblog.com/post/2015-11-03-loss-developments-via-growth-curves-and/)
- [PK/PD reserving models - Markus Gesmann](https://magesblog.com/post/2018-01-30-pkpd-reserving-models/)
- [Hierarchical compartmental reserving models - Markus Gesmann](https://magesblog.com/post/hierarchical-compartmental-reserving-models/)
- [CAS Monograph No. 1 - Stochastic Loss Reserving using Bayesian MCMC Models, Glenn Meyers](https://www.casact.org/pubs/monographs/papers/01-Meyers.PDF)
- [PrObEx - SCOR Paper No10](https://www.scor.com/sites/default/files/sp10.pdf)
- [PrObEx and Internal Model - Calibrating dependencies among risks in Non-Life](https://idei.fr/sites/default/files/medias/doc/conf/scor/idei_paris_012014/slides_conf_scor/canestraro_davide.pdf)
- [Severity Curve Fitting for Long Tailed Lines: An Application of Stochastic Processes and Bayesian Models, Greg McNulty, 2018](https://www.variancejournal.org/articlespress/articles/Severity-McNulty.pdf)
- [Introduction to Bayesian Loss Development](https://www.casact.org/pubs/forum/16sforum/Clark.pdf)
- [Bayesian Claim Severity with Mixed Distributions - Escoto](http://www.variancejournal.org/issues/07-02/110.pdf)
- [A Multivariate Bayesian Claim Count Development Model With Closed Form Posterior and Predictive Distributions Mildenhall, 2006](https://www.casact.org/pubs/forum/06wforum/06w455.pdf)
- [A Course in Credibility Theory and its Applications, Hans Bühlmann, Alois Gisler](https://www.amazon.co.uk/dp/3540257535)

## Tooling

### Stan
- [R/Stan installation instructions](https://github.com/stan-dev/rstan/wiki/RStan-Getting-Started)
- Eric's [old receipe for R/Stan on Windows](https://gist.github.com/ericnovik/ff7daab5c3eb0c8396887110a9dbd6ac)
- [Introduction to Stan](https://rawgithub.com/InsuranceDataScience/StanWorkshop2018/master/ericnovik/stan_man_1.html) (Eric Novik)

### BRMS
- [From classical GLMs to Bayesian multi-level models](https://github.com/InsuranceDataScience/StanWorkshop2018/blob/master/paul_buerkner/From_GLMs_to_MLMs.pdf) (Paul Bürkner)

### PYMC3

Project [website](https://docs.pymc.io/)

[Bayesian Analysis with Python: Introduction to statistical modeling and probabilistic programming using PyMC3 and ArviZ, 2nd Edition Paperback – 26 Dec 2018 by Osvaldo Martin](https://www.amazon.co.uk/dp/1789341655/?coliid=I2MIA7LBPRE6F0&colid=2NFXBRCJ4YHNS&psc=0&ref_=lv_ov_lig_dp_it)

### Other tools

BUGS, WinBUGs, JAGS, Pystan


### pymc3 questions

- importance of GPU processing

## Model Notes

### McNulty Method

- individual claim paths not clear from data
- quite complex
- doesn't tell much about how individual claims might be expected to develop
- fake data
- some of priors look suspiciously detailed

## Datasets

### CAS Loss Simulation Model

Not a Bayesian method but potentially useful for testing or for thinking about the claims generation process.

[Link](https://www.casact.org/research/lsmwp/index.cfm?fa=software)

### CAS LOSS RESERVING DATA PULLED FROM NAIC SCHEDULE P

Used in Glenn Meyers monograph.

[link](https://www.casact.org/research/index.cfm?fa=loss_reserves_data)
