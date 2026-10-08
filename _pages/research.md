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
  margin-top: 0.5em;
  font-size: 0.88em;
  line-height: 1.5;
  color: #555;
}

.paper-abstract summary {
  cursor: pointer;
  font-weight: 600;
  color: #333;
  margin-bottom: 0.35em;
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
      <span class="paper-date">(September 2026)</span>
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
      <span class="paper-date">(December 2025)</span>
    </div>

    <div class="paper-status">
      Revise and resubmit, <em>International Statistical Review</em> |
      <a href="https://arxiv.org/abs/2510.22714" target="_blank" rel="noopener noreferrer">arXiv</a>
    </div>

    <details class="paper-abstract">
      <summary>Abstract</summary>

      <p>
        We provide pairwise-difference (Gini-type) representations of higher-order central moments for both general random variables and empirical moments. Such representations do not require a measure of location. For third and fourth moments, this yields pairwise-difference representations of skewness and kurtosis coefficients. We show that all central moments possess such representations, so no reference to the mean is needed for moments of any order. This is done by considering i.i.d. replications of the random variables considered, by observing that central moments can be interpreted as covariances between a random variable and powers of the same variable, and by giving recursions which link the pairwise-difference representation of any moment to lower-order ones. Numerical summation identities are deduced. Through a similar approach, we give analogues of the Lagrange and Binet–Cauchy identities for general random variables, along with a simple derivation of the classic Cauchy–Schwarz inequality for covariances. Finally, an application to unbiased estimation of centered moments is discussed.
      </p>
    </details>
  </li>

  <li class="paper-item">
    <div>
      <span class="paper-title">“From Announcement Reactions to Macroeconomic Effects: Identification-Robust Inference with Weakly Separated Policy and Information Shocks”</span>,
      <span class="paper-authors">
        with
        <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html" target="_blank" rel="noopener noreferrer">Jean-Marie Dufour</a>
      </span>
      <span class="paper-date">(September 2026)</span>
    </div>

    <details class="paper-abstract">
      <summary>Abstract</summary>

      <p>
        Market reactions to FOMC announcements reflect both unexpected monetary-policy actions and information about the economic outlook. Because these forces can generate different macroeconomic responses, separating them is essential for measuring policy transmission. Empirical work typically constructs shock-specific proxies from high-frequency financial price movements and then uses their monthly aggregates as external instruments in proxy SVARs. We show that this two-step strategy faces two distinct identification problems: weak shock separation upstream, when announcement-window data do not distinguish the latent shocks, and weak proxy relevance downstream, when a correctly separated proxy is only weakly correlated with its target SVAR shock. Standard weak-instrument methods address the second problem, not the first.
      </p>

      <p>
        Using identification through heteroskedasticity in the upstream model, we show that nearly proportional covariance changes across announcement states can leave the policy-information shocks weakly separated. The generated proxy can then remain a mixture of structural shocks, invalidating downstream plug-in inference, including Anderson–Rubin procedures. We develop joint inference procedures that incorporate proxy construction directly into structural inference. A projected Stock–Wright-type procedure remains valid under weak upstream separation and weak downstream relevance, while a reduced-profile procedure is sharper under an additional conditional-rank condition. Monte Carlo experiments show severe overrejection by plug-in methods and size control by joint inference. In an FOMC application, expanding the measurement window beyond the policy statement substantially strengthens the measured central-bank-information signal, while yielding little scale-adjusted improvement for the monetary-policy proxy. Yet dynamic macroeconomic effects remain imprecisely identified. Stronger measured proxies therefore need not deliver more reliable structural inference.
      </p>
    </details>
  </li>

</ol>

<h2>Work in Progress</h2>

<ol class="paper-list">

  <li class="paper-item">
    <div>
      <span class="paper-title">“Finite-Sample Inference for High-Frequency Jump Tests under Market Microstructure Frictions”</span>,
      <span class="paper-authors">
        with Md. Nazmul Ahsan and
        <a href="https://jeanmariedufour.research.mcgill.ca/dufour.html" target="_blank" rel="noopener noreferrer">Jean-Marie Dufour</a>
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
      2026 JSM Proceedings
    </div>
  </li>

</ol>

</div>
