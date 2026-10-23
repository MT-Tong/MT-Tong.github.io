---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

<style>
.research-page {
  counter-reset: paper-counter;
}

.paper-list {
  list-style: none;
  padding-left: 0;
  margin-bottom: 2.2em;
}

.paper-item {
  counter-increment: paper-counter;
  margin-bottom: 1.8em;
  padding-left: 2.4em;
  position: relative;
}

.paper-item::before {
  content: counter(paper-counter) ".";
  position: absolute;
  left: 0;
  font-weight: bold;
}

.paper-title {
  font-weight: 700;
  font-size: 1.05em;
  line-height: 1.35;
}

.paper-authors,
.paper-date {
  display: inline;
  font-size: 0.95em;
}

.paper-status {
  margin-top: 0.25em;
  font-size: 0.92em;
  font-style: italic;
}

.paper-abstract {
  margin-top: 0.6em;
  font-size: 0.88em;
  line-height: 1.5;
  color: #000;
}

.paper-abstract summary {
  cursor: pointer;
  font-weight: 600;
  color: inherit;
  margin-bottom: 0.35em;
}

html[data-theme="dark"] .paper-abstract {
  color: #fff;
}

.paper-abstract p {
  margin-top: 0.4em;
}
</style>

<div class="research-page">

<h2>Job Market Paper</h2>

<ol class="paper-list">

  <li class="paper-item">
    <div>
      <span class="paper-title">“Estimating Higher-Order Stochastic Volatility Models with Moving-Average Components: Methodology and Applications”</span>,
      <span class="paper-authors">
        with
        <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html" target="_blank" rel="noopener noreferrer">Jean-Marie Dufour</a>
      </span>
      <span class="paper-date">(September 2026, 84 pages)</span>
    </div>

    <details class="paper-abstract">
      <summary>Abstract</summary>

      <p>
        Moving-average dynamics provide a parsimonious way to capture short-run time-series patterns that may otherwise require additional autoregressive lags. Yet they are rarely incorporated into stochastic volatility models because latent volatility complicates estimation and model selection. We develop a framework for a broad class of stochastic volatility models in which latent log-volatility follows an ARMA(p,q) process, denoted SV(p,q). For this class of models, we show that appropriately transformed returns admit an ARMA representation. The proposed estimation procedure then consists of two steps: it first estimates the ARMA parameters by regression and then recovers the structural parameters through autocovariance matching. Consistency and asymptotic normality are established for the regression estimator. To guide empirical implementation, we develop a two-stage procedure for selecting the model orders. Monte Carlo simulations assess the method’s finite-sample performance. In an application to daily S&amp;P 500 returns from 1962 to 2024, the model-selection procedure favors an SV(1,1) specification, supporting the inclusion of a moving-average component in latent volatility. The empirical analysis also evaluates volatility forecasts at multiple horizons against standard GARCH-family benchmarks. Together, these contributions provide a practical framework for estimation, model selection, and forecasting with richer volatility dynamics.
      </p>
    </details>
  </li>

</ol>

<h2>Working Papers</h2>

<ol class="paper-list">

  <li class="paper-item">
    <div>
      <span class="paper-title">“Pairwise Difference Representations of Moments: Gini and Generalized Lagrange Identities”</span>,
      <span class="paper-authors">
        with
        <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html" target="_blank" rel="noopener noreferrer">Jean-Marie Dufour</a>
        and Abderrahim Taamouti
      </span>
      <span class="paper-date">(September 2026, 26 pages)</span>
    </div>

    <div class="paper-status">
      Submitted to <em>Communications in Statistics - Theory and Methods</em> |
      <a href="https://arxiv.org/abs/2510.22714" target="_blank" rel="noopener noreferrer">arXiv</a>
    </div>

    <details class="paper-abstract">
      <summary>Abstract</summary>

      <p>
        We provide pairwise-difference (Gini-type) representations of higher-order central moments for both general random variables and empirical moments. Such representations do not require a measure of location. For third and fourth moments, this yields pairwise-difference representations of skewness and kurtosis coefficients. We show that all central moments possess such representations, so no reference to the mean is needed for moments of any order. This is done by considering i.i.d. replications of the random variables considered, by observing that central moments can be interpreted as covariances between a random variable and powers of the same variable, and by giving recursions that link the pairwise-difference representation of any moment to lower-order ones.
      </p>
    </details>
  </li>

  <li class="paper-item">
    <div>
      <span class="paper-title">“From Announcement Reactions to Macroeconomic Effects: Identification-Robust Inference with Weakly Separated Policy and Information Shocks”</span>.
      <span class="paper-date">(September 2026, 85 pages)</span>
    </div>

    <details class="paper-abstract">
    <summary>Abstract</summary>

    <p>
      Market reactions to FOMC announcements reflect both unexpected monetary-policy actions and information about the economic outlook. Empirical studies construct shock-specific proxies from high-frequency financial price movements around policy announcements, aggregate them to monthly frequency, and use them as external instruments in structural vector autoregressions to estimate dynamic macroeconomic effects. This strategy faces two identification problems: weak shock separation upstream, when announcement data do not clearly distinguish the latent shocks, and weak proxy relevance downstream, when a correctly separated proxy is weakly correlated with its target shock. Standard weak-instrument methods address the second problem, not the first. Using identification through heteroskedasticity, we show that weak separation can leave generated proxies as mixtures of structural shocks, invalidating plug-in inference, including Anderson–Rubin procedures. We develop joint inference that incorporates proxy construction directly into structural inference. A projected procedure remains asymptotically valid under weak upstream separation and weak downstream relevance, while a reduced-profile procedure is sharper under additional conditional identification and regularity conditions. Monte Carlo experiments show severe overrejection by plug-in methods, while the joint procedures avoid this distortion in the designs considered. In an FOMC application, extending the measurement window from the policy statement to include the press conference appears to sharpen inference about central-bank-information shocks when the estimated proxies are treated as fixed. Once proxy-construction uncertainty is incorporated, however, the corresponding confidence sets become unbounded, and most dynamic macroeconomic effects remain imprecisely determined. Broader announcement coverage therefore need not deliver more precise inference about macroeconomic transmission.
  </p>
</details>
  </li>

</ol>

<h2>Conference Proceedings</h2>

<ol class="paper-list">

  <li class="paper-item">
    <div>
      <span class="paper-title">“Pairwise Difference Representations of Central Moments: Skewness, Kurtosis, and Higher-Order Recursions”</span>,
      <span class="paper-authors">
        with
        <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html" target="_blank" rel="noopener noreferrer">Jean-Marie Dufour</a>
        and Abderrahim Taamouti
      </span>
    </div>

    <div class="paper-status">
      2025 JSM Proceedings, 15 pages |
      <a href="https://doi.org/10.5281/zenodo.17379223" target="_blank" rel="noopener noreferrer">DOI</a>
    </div>
  </li>

</ol>

<h2>Work in Progress</h2>

<ol class="paper-list">

  <li class="paper-item">
    <div>
      <span class="paper-title">“Simulation-Based High-Frequency Jump Tests”</span>,
      <span class="paper-authors">
        with Md. Nazmul Ahsan
      </span>
    </div>
  </li>

  <li class="paper-item">
    <div>
      <span class="paper-title">“High-Dimensional Stochastic Covariance Estimation via Model Aggregation”</span>,
      <span class="paper-authors">
        with Md. Nazmul Ahsan and
        <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html" target="_blank" rel="noopener noreferrer">Jean-Marie Dufour</a>
      </span>
    </div>
  </li>

</ol>

</div>
