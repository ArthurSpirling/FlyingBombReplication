# Replication Materials for "The Flying Bomb and the Actuary"

In the 2019 edition of [*Signifance*](https://www.significancemagazine.com/), Luke Shaw and Liam Shaw have an interesting article on so-called flying bombs from the Second World War.  Specifically, Shaw and Shaw study the bombing of London, by German [V1 'doodlebugs'](https://en.wikipedia.org/wiki/V-1_flying_bomb)  and [V2 rockets](https://en.wikipedia.org/wiki/V-2_rocket).  These were especially common in South London, and many fell in my hometown of [Carshalton](https://www.bbc.co.uk/history/ww2peopleswar/stories/15/a2099315.shtml).

The authors revisit earlier work by RD Clarke, an actuary and statistician.  His interest was in whether the bombs were targeted, or fell 'randomly'. In his original article (["An application of the Poisson distribution"](https://www.cambridge.org/core/journals/journal-of-the-institute-of-actuaries/article/an-application-of-the-poisson-distribution/F75111847FDA534103BD4941BD96A78E), 1946) Clarke used the Poisson distribution as a null hypothesis. His method was to uniformly divide a map of (south) London into equal unit squares of land, and then count the number of V1 bombs that landed in each.  If these counts are Poisson distributed, this is *prima facie* evidence that the bombs were **not** targeted at specific places on the map.  That is, the way the bombs fell is consistent with what we would expect if they were dropped randomly.

# R code
In April 2021, I set out to replicate what the authors had done in the paper (which includes a replcation of Clarke). I noticed some discrepencies between my results, what is written in the paper and what the authors (helpfully) provided in their [replication archive](https://lukefshaw.netlify.app/the-flying-bomb-and-the-actuary-supplementary-analysis/).  In an email exchange, the authors agreed that what follows below is correct---at least in terms of the subset of results I replicated.  

## Figure 1: Clarke's original analysis


