--- 
title: "*Doing Bayesian Data Analysis* in brms and the tidyverse"
subtitle: "version 0.1.0"
author: ["A Solomon Kurz"]
date: "2020-02-17"
site: bookdown::bookdown_site
output: bookdown::gitbook
documentclass: book
geometry:
  margin = 0.5in
urlcolor: blue
highlight: tango
header-includes:
  \usepackage{underscore}
  \usepackage[T1]{fontenc}
link-citations: yes
github-repo: ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse
twitter-handle: SolomonKurz
description: "This project is an attempt to re-express the code in Kruschke's (2015) textbook. His models are re-fit in brms, plots are redone with ggplot2, and the general data wrangling code predominantly follows the tidyverse style."
---

# What and why {-}

Kruschke began his text with "This book explains how to actually do Bayesian data analysis, by real people (like you), for realistic data (like yours)." In the same way, this project is designed to help those real people do Bayesian data analysis. My contribution is converting Kruschke's JAGS and Stan code for use in Bürkner's [**brms** package](https://github.com/paul-buerkner/brms), which makes it easier to fit Bayesian regression models in **R** using Hamiltonian Monte Carlo (HMC). I also prefer plotting and data wrangling with the packages from the [**tidyverse**](http://style.tidyverse.org). So we'll be using those methods, too.

This project is not meant to stand alone. It's a supplement to the second edition of [Kruschke's *Doing Bayesian Data Analysis*](https://sites.google.com/site/doingbayesiandataanalysis/). Please give the source material some love.

## Caution: Work in progress {-}

### We've come so far! {-}

The first phase for this project was focused on developing the primary content, a few chapters at a time. Welcome to version 0.1.0 and the beginning of a new project phase! With version 0.1.0, we now have [fairly] complete drafts of all chapters in Kruschke's text. The supermajority of Kruschke's JAGS and Stan models have been fit using **brms** code and most of the results are quite comparable to those in the original text. We have also reproduced most of the data-related figures and tables and little subpoints and examples sprinkled throughout Kruschke's prose. In addition, we have a few bonus content areas not found in the original text, such as

* an introduction to Bayesian information criteria in Section 10.3.2,
* an extra walkout of simple effect sizes in Section 19.6, and
* a comparison of the hierarchical aggregated binomial model with Kruschke’s hierarchical Poisson approach in Section 24.4.

Another nice feature of this version is all models have ben refit with **brms** 2.11.5 and saved as external files you can access in the [`fits` folder on GitHub](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/tree/master/fits).

### We're not done yet and I could use your help. {-}

There are some minor improvements I'd like to add in future versions, such as refreshed hyperlinks (e.g., prioritizing HTTPS, following canonical CRAN style), prettying up the plots with custom themes, and so on. As much as I'm looking forward to these improvements, they're mainly just fluff. The most important improvements I'd like to make are patching up the content holes. A few simulations, figures, and models are beyond my current skill set. I’ve opened separate GitHub issues for the most important ones and they are as follows:

* the random-walk simulation in Section 7.2.3 and the corresponding plot in Figure 7.3 ([issue #14](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/14)),
* the effective-sample-size simulations in Section 7.5.2 and the corresponding plots in Figures 7.13 and 7.14 ([issue #15](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/15)),
* several of the simulations in Sections 11.1.4, 11.3.1, and 11.3.2 and their corresponding figures (issues [#16](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/16), [#17](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/17), [#18](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/18), and [#19](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/19)),
* the stopping-rule simulations in Section 13.3.2 and their corresponding figures ([issue #20](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/20)),
* the data necessary to properly reproduce the HMC proposal schematic presented in Section 14.1 and Figures 14.1 through 14.3 ([issue #21](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/21)), and
* the conditional logistic models of Section 22.3.3.2 ([issue #22](https://github.com/ASKurz/Doing-Bayesian-Data-Analysis-in-brms-and-the-tidyverse/issues/22)).

If you know how to conquer any of these unresolved challenges, I'd love to hear all about it. In addition, please feel free to open a new issue if you find any flaws in the other sections of the project.

## Thank-you's are in order {-}

Before we enter the primary text, I'd like to thank the following for their helpful contributions:

* Paul-Christian Bürkner ([\@paul-buerkner](https://github.com/paul-buerkner)),
* Andrew Gelman ([\@andrewgelman](https://github.com/andrewgelman)),
* Matthew Kay ([\@mjskay](https://github.com/mjskay)),
* TJ Mahr ([\@tjmahr](https://github.com/tjmahr)),
* Lukas Neugebauer ([\@LukasNeugebauer](https://github.com/LukasNeugebauer)),
* Demetri Pananos ([\@Dpananos](https://github.com/dpananos)),
* Aki Vehtari ([\@avehtari](https://github.com/avehtari)),
* Matti Vuorre ([\@mvuorre](https://github.com/mvuorre)), and
* Brenton M. Wiernik ([\@bwiernik](https://github.com/bwiernik)).



