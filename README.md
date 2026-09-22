# justification
Code and data for _On the justification for sampling-based statistics in randomised experiments_.

[![DOI](https://zenodo.org/badge/1369749855.svg)](https://doi.org/10.5281/zenodo.22898968)

## Open peer review
This article (`justification.pdf`) has been submitted to _Meta-Psychology_. 
Participate in open peer review by sending an email to open.peer.reviewer@gmail.com. 
The full editorial process of all articles under review at Meta-Psychology can be found following this link:

https://tinyurl.com/mp-submissions

You will find this preprint by searching for the first author's name (i.e., Vanhove).

## Abstract
When popular statistical tools such as the _t_-test are taught, 
the narrative is one in which the data are sampled randomly from some population.
Real studies employing random sampling are, however, much rarer than the
ubiquity of these tools would suggest, and students may wonder
what justifies their use in the absence of random sampling or even
of a clear notion of what the population might be.
Reassuringly, some of these tools can be understood in an altogether
more common setting: experiments in which units are randomly assigned to conditions.
This perspective clarifies why familiar procedures such as the _t_-test
tend to perform reasonably well in randomised experiments,
which may go some way towards explaining the slow uptake of inferential
methods explicitly derived from random assignment rather than random sampling.
At the same time, it underscores a difference in the scope of inference 
afforded by random sampling versus random assignment.
Furthermore, this perspective foregrounds flexible randomisation-based methods,
whose validity follows directly from the study design and which, as I suggest,
provide a natural starting point for teaching statistical inference to non-mathematicians.

## Data
The data stems from Klein et al.'s (2014) [_Investigating variation in replicability: A "many labs" replication project_](https://doi.org/10.1027/1864-9335/a000178)
and were made available under the CC0 1.0 Universal license on [OSF.io](https://osf.io/8cd4r).
The file `Klein2014_brasilia_gambler.csv`, which contains the data on the gambler's fallacy experiment from the Brasília sample was extracted from this dataset, and is made available here under the same license.

The data set contains three columns and 114 observations:

* `Sample`: always `brasilia`.
* `Condition`: `two6` if the participants had to imagine two sixes were rolled, `three6` if three sixes.
* `RollsImagined`: the number of prior rolls they estimated must have occurred.

## Code
The R code is embedded in the `justification.Rmd` file. The following software versions were used:

<code>
  > devtools::session_info("attached")
  ─ Session info ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
   setting  value
   version  R version 4.6.1 (2026-06-24 ucrt)
   os       Windows 11 x64 (build 26200)
   system   x86_64, mingw32
   ui       RStudio
   language (EN)
   collate  English_United Kingdom.utf8
   ctype    English_United Kingdom.utf8
   tz       Europe/Zurich
   date     2026-09-22
   rstudio  2026.08.1+195 Yellow Yarrow (desktop)
   pandoc   3.8.3 @ C:/Program Files/RStudio/resources/app/bin/quarto/bin/tools/ (via rmarkdown)
   quarto   1.9.38 @ C:\\Users\\VanhoveJ\\AppData\\Local\\Programs\\Quarto\\bin\\quarto.exe
  
  ─ Packages ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
   package   * version date (UTC) lib source
   dplyr     * 1.2.1   2026-04-03 [1] CRAN (R 4.6.1)
   forcats   * 1.0.1   2025-09-25 [1] CRAN (R 4.6.1)
   ggplot2   * 4.0.3   2026-04-22 [1] CRAN (R 4.6.1)
   lubridate * 1.9.5   2026-02-04 [1] CRAN (R 4.6.1)
   purrr     * 1.2.2   2026-04-10 [1] CRAN (R 4.6.1)
   readr     * 2.2.0   2026-02-19 [1] CRAN (R 4.6.1)
   stringr   * 1.6.0   2025-11-04 [1] CRAN (R 4.6.1)
   tibble    * 3.3.1   2026-01-11 [1] CRAN (R 4.6.1)
   tidyr     * 1.3.2   2025-12-19 [1] CRAN (R 4.6.1)
   tidyverse * 2.0.0   2023-02-22 [1] CRAN (R 4.6.1)
</code>
