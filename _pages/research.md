---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

<style>
.paper-list {
  list-style: none;
  padding-left: 0;
  margin-bottom: 2.2em;
}

.paper-item {
  margin-bottom: 1.8em;
  scroll-margin-top: 5rem;
}

.paper-title {
  font-weight: 700;
  font-size: 1.05em;
  line-height: 1.35;
}

.paper-authors,
.paper-meta,
.paper-status {
  margin-top: 0.2em;
  font-size: 0.95em;
  line-height: 1.45;
}

.paper-abstract {
  margin-top: 0.5em;
  font-size: 0.88em;
  line-height: 1.5;
  color: #000;
}

.paper-abstract summary {
  cursor: pointer;
  width: fit-content;
  font-weight: 600;
  color: inherit;
}

.paper-abstract[open] summary {
  margin-bottom: 0.35em;
}

.paper-abstract p {
  margin-top: 0.4em;
}

html[data-theme="dark"] .paper-abstract {
  color: #fff;
}
</style>

<div class="research-page">

<h2>Job Market Paper</h2>

<ul class="paper-list">

  <li class="paper-item" id="job-market-paper">

    <div class="paper-title">
      “Estimating Higher-Order Stochastic Volatility Models with Moving-Average Components: Methodology and Applications”
    </div>

    <div class="paper-authors">
      with
      <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html"
         target="_blank"
         rel="noopener noreferrer">Jean-Marie Dufour</a>
    </div>

    <div class="paper-meta">
      (September 2026; Main: 37 pages; Appendix: 43 pages). Submitted.
    </div>

    <details class="paper-abstract" open>
      <summary>Abstract</summary>

      <p>
        Moving-average dynamics provide a parsimonious way to capture short-run time-series patterns that may otherwise require additional autoregressive lags. Yet they are rarely incorporated into stochastic volatility models because latent volatility complicates estimation and model selection. We develop a framework for a broad class of stochastic volatility models in which latent log-volatility follows an ARMA(p,q) process, denoted SV(p,q). For this class of models, we show that appropriately transformed returns admit an ARMA representation. The proposed estimation procedure then consists of two steps: it first estimates the ARMA parameters by regression and then recovers the structural parameters through autocovariance matching. Consistency and asymptotic normality are established for the regression estimator. To guide empirical implementation, we develop a two-stage procedure for selecting the model orders. Monte Carlo simulations assess the method’s finite-sample performance. In an application to daily S&amp;P 500 returns from 1962 to 2024, the model-selection procedure favors an SV(1,1) specification, supporting the inclusion of a moving-average component in latent volatility. The empirical analysis also evaluates volatility forecasts at multiple horizons against standard GARCH-family benchmarks. Together, these contributions provide a practical framework for estimation, model selection, and forecasting with richer volatility dynamics.
      </p>
    </details>

  </li>

</ul>

<h2>Working Papers</h2>

<ul class="paper-list">

  <li class="paper-item">

    <div class="paper-title">
      “Gini Representations of Skewness, Kurtosis and Higher-Order Moments”
    </div>

    <div class="paper-authors">
      with
      <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html"
         target="_blank"
         rel="noopener noreferrer">Jean-Marie Dufour</a>
      and Abderrahim Taamouti
    </div>

    <div class="paper-meta">
      (September 2026; 26 pages).
    </div>

    <div class="paper-status">
      Submitted to <em>Communications in Statistics - Theory and Methods</em> |
      <a href="https://arxiv.org/abs/2510.22714"
         target="_blank"
         rel="noopener noreferrer">arXiv</a>
    </div>

    <details class="paper-abstract">
      <summary>Abstract</summary>

      <p>
        We provide pairwise-difference (Gini-type) representations of higher-order central moments for both general random variables and empirical moments. Such representations do not require a measure of location. For third and fourth moments, this yields pairwise-difference representations of skewness and kurtosis coefficients. We show that all central moments possess such representations, so no reference to the mean is needed for moments of any order. This is done by considering i.i.d. replications of the random variables considered, by observing that central moments can be interpreted as covariances between a random variable and powers of the same variable, and by giving recursions that link the pairwise-difference representation of any moment to lower-order ones.
      </p>
    </details>

  </li>

  <li class="paper-item">

    <div class="paper-title">
      “From Announcement Reactions to Macroeconomic Effects: Identification-Robust Inference with Weakly Separated Policy and Information Shocks”
    </div>

    <div class="paper-meta">
      (September 2026; Main: 38 pages; Appendix: 42 pages).
    </div>

    <details class="paper-abstract">
      <summary>Abstract</summary>

      <p>
        Market reactions to FOMC announcements reflect both unexpected monetary policy actions and information about the economic outlook. Empirical studies construct shock-specific proxies from high-frequency financial price movements around policy announcements, aggregate them to monthly frequency, and use them as external instruments in structural vector autoregressions to estimate dynamic macroeconomic effects. This strategy faces two identification problems: weak shock separation upstream, when announcement data do not clearly distinguish the latent shocks, and weak proxy relevance downstream, when a correctly separated proxy is weakly correlated with its target shock. Standard weak-instrument methods address the second problem, not the first. Using identification through heteroskedasticity, we show that weak separation can leave generated proxies as mixtures of structural shocks, invalidating plug-in inference, including Anderson–Rubin procedures. We develop joint inference that incorporates proxy construction directly into structural inference. A projected procedure remains asymptotically valid under weak upstream separation and weak downstream relevance, while a reduced-profile procedure is sharper under additional conditional identification and regularity conditions. Monte Carlo experiments show severe overrejection by plug-in methods, while the joint procedures avoid this distortion in the designs considered. In an FOMC application, extending the measurement window from the policy statement to include the press conference appears to sharpen inference about central bank information shocks when the estimated proxies are treated as fixed. Once proxy-construction uncertainty is incorporated, however, the corresponding confidence sets become unbounded, and most dynamic macroeconomic effects remain imprecisely determined. Broader announcement coverage therefore need not deliver more precise inference about macroeconomic transmission.
      </p>
    </details>

  </li>

</ul>

<h2>Conference Proceedings</h2>

<ul class="paper-list">

  <li class="paper-item">

    <div class="paper-title">
      “Pairwise Difference Representations of Central Moments: Skewness, Kurtosis, and Higher-Order Recursions”
    </div>

    <div class="paper-authors">
      with
      <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html"
         target="_blank"
         rel="noopener noreferrer">Jean-Marie Dufour</a>
      and Abderrahim Taamouti
    </div>

    <div class="paper-meta">
      (October 2025; 15 pages).
    </div>

    <div class="paper-status">
      <em>2025 Joint Statistical Meetings (JSM) Proceedings</em> |
      <a href="https://doi.org/10.5281/zenodo.17379223"
         target="_blank"
         rel="noopener noreferrer">DOI</a>
    </div>

  </li>

</ul>

<h2>Work in Progress</h2>

<ul class="paper-list">

  <li class="paper-item">

    <div class="paper-title">
      “Simulation-Based High-Frequency Jump Tests”
    </div>

    <div class="paper-authors">
      with Md. Nazmul Ahsan
    </div>

  </li>

  <li class="paper-item">

    <div class="paper-title">
      “High-Dimensional Stochastic Covariance Estimation via Model Aggregation”
    </div>

    <div class="paper-authors">
      with Md. Nazmul Ahsan and
      <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html"
         target="_blank"
         rel="noopener noreferrer">Jean-Marie Dufour</a>
    </div>

  </li>

</ul>

</div>
