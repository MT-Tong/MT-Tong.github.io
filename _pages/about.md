---
permalink: /
title: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% include base_path %}

Welcome! I am a PhD candidate in Economics at McGill University in Canada.

My research interests lie at the intersection of financial econometrics, macroeconometrics, and time-series analysis. I develop econometric methods that use financial data to learn about financial risks and economic shocks that cannot be observed directly. My work focuses on how financial risk evolves, how different shocks shape market reactions, and how their effects propagate through the broader economy. These methods support more reliable risk measurement, forecasting, and macroeconomic policy evaluation.

You can find my [CV here]({{ base_path }}/files/CV.pdf) and more details about my ongoing projects on my [Research page]({{ base_path }}/research/).

***I am on the 2026–2027 Job Market!***

## Job Market Paper

<style>
.homepage-paper {
  margin-bottom: 1.8em;
}

.homepage-paper-title {
  font-weight: 700;
  font-size: 1.05em;
  line-height: 1.35;
}

.homepage-paper-authors {
  margin-top: 0.2em;
  font-size: 0.9em;
}

.homepage-paper-abstract {
  margin-top: 0.6em;
  font-size: 0.88em;
  line-height: 1.5;
  color: #555;
}

.homepage-paper-abstract summary {
  cursor: pointer;
  font-weight: 600;
  color: #333;
  margin-bottom: 0.35em;
}

.homepage-paper-abstract p {
  margin-top: 0.5em;
}
</style>

<div class="homepage-paper">

  <div class="homepage-paper-title">
    “Estimating Higher-Order Stochastic Volatility Models with Moving-Average Components: Methodology and Applications”
  </div>

  <div class="homepage-paper-authors">
    with
    <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html" target="_blank" rel="noopener noreferrer">Jean-Marie Dufour</a>
  </div>

  <details class="homepage-paper-abstract">
    <summary>Abstract</summary>

    <p>
      Moving-average dynamics provide a parsimonious way to capture short-run time-series patterns that may otherwise require additional autoregressive lags. Yet they are rarely incorporated into stochastic volatility models because latent volatility complicates estimation and model selection. We develop a framework for a broad class of stochastic volatility models in which latent log-volatility follows an ARMA(p,q) process, denoted SV(p,q). For this class of models, we show that appropriately transformed returns admit an ARMA representation. The proposed estimation procedure then consists of two steps: it first estimates the ARMA parameters by regression and then recovers the structural parameters through autocovariance matching. Consistency and asymptotic normality are established for the regression estimator. To guide empirical implementation, we develop a two-stage procedure for selecting the model orders. Monte Carlo simulations assess the method’s finite-sample performance. In an application to daily S&amp;P 500 returns from 1962 to 2024, the model-selection procedure favors an SV(1,1) specification, supporting the inclusion of a moving-average component in latent volatility. The empirical analysis also evaluates volatility forecasts at multiple horizons against standard GARCH-family benchmarks. Together, these contributions provide a practical framework for estimation, model selection, and forecasting with richer volatility dynamics.
    </p>
  </details>

</div>

Please feel free to contact me at [meilin.tong@mail.mcgill.ca](mailto:meilin.tong@mail.mcgill.ca).


