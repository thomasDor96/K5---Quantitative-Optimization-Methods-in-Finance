# Time Series Models: Basics


## Definitions
*stochastic process* is a sequence of random variables and can be viewed as the "theortical" or "population" analog of a time series- conversely, a time series can be considered a sample from a stochastic process. "stochastic" is a synonym for random. One of the most useful methods for obtaining parsimony in a time series model, is to assume some form of distributional invariance over time, or *stationarity*, a property discussed next.


## Stationary Process
When we observe a time series, the fluctuations appear to be random, but often with the sample type of stochastic behaviour from one time period to the next. For example, returns on stocks or changes in interest rates can be very different from the previous year, but the mean, standard deviation, and other statistical propertities often are similar from one year to the next. Similarly, the demand for many consumer products, such as sunscreen, winter coats, and electricity, has random as well as seasonal variation, but each summer is similar to the past summer, each winter to poast winter, at least over shorter time periods. Stationary stochastic proecesses are rpobability models for time series with time-invariant behavior. \newline

A process is said to be *strictly stationary* if all aspects of its behavior are unchanged by shifts in time. Mathematically, stationarity is defined as the requirement that for every *m* and *n*, the distributions of $(Y_1, \dots, Y_n)$ and $(Y_{1+m}, \dots, Y_{n+m})$ are the same; that is, the probability distribution of a sequence of $n$ ovservations does not depend on their time origin. Strict stationarity is a very strong assumption, because it requires that "all aspects" of stochastic behaviour be constant in time. Often, it will be suffice to assume less, namely, weak stationarity. A process is *weakly stationary* if its mean, variance and covariance are unchanged by time shifts. More precisely, $Y_1, Y_2,\dots$ is a *weakly stationary process* if:

* $E(Y_t)$ = \mu (a finite constant) for all t
* $Var(Y_t) = \sigma^2$ (a positive finite constant) for all t; and
* $Cov(Y_t, Y_s) = \gamma(|t - s|)$ for all t and s for some function $\gamma(h)$.

Thus, the mean and variance do not change with time and the covariance between two observations depends only on the *lag*, the time distance $|t - s|$ between them, not the indices *t* and *s* directly. For example, if the process is weakly stationary, then the covariance between $Y_2$ and $Y_5$ is the same as the covariance between $Y_7$ and $Y_10$, since each pair is seperated by three units of time. The adjective "weakly" in "weakly stationary" refers to the fact that we are only assuming that means, variance, and covariances, not other distributional characteristics such as quantiles, skewness, and kurtosis, are stationary.



