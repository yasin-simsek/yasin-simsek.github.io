---
layout: default
title: "Research"
---

<style>
.abstract-toggle {
    text-decoration: none; /* Removes underline */
    cursor: pointer;
    color: #012169;
}

.abstract-content {
    display: none;           /* Hide abstract by default */
    opacity: 0;
    transition: opacity 0.3s ease-in-out;
}

.abstract-content.show {
    display: inline-block;   /* Show abstract when .show is added */
    opacity: 1;
    transition: opacity 0.3s ease-in-out;
}

.no-underline {
    text-decoration: none; /* Removes underline */
    color: #012169; /* Keeps the original color */
    cursor: pointer; /* Makes it clear it's clickable */
}

.no-underline:hover {
    text-decoration: underline; /* Optional: Add underline on hover */
    color: #012169; /* Optionally change the color */
}

.abstract-toggle:hover {
    text-decoration: underline; /* Optional: Add underline on hover */
}

.middot {
    font-size: 2.0em;        /* Increase the size */
    margin: 0 10px;          /* Space around the dot */
    line-height: 1;          /* Ensures the line height matches text size */
    vertical-align: middle;  /* Aligns the dot with the text baseline */
    position: relative;      /* Ensures fine control over positioning */
    top: -0.1em;             /* Fine-tune vertical position to center */
}

</style>


#### <span style="color: #012169;">Job Market Paper</span>

[**Beyond Returns: A Candlestick-Based Approach to Spot Covariance Estimation**](assets/documents/jmp_last_version.pdf) *(updated frequently)*
<br> 
<span class="abstract-toggle" onclick="toggleAbstract(this)">Abstract</span> 
<span class="abstract-content"> *Spot covariance estimation is commonly based on high-frequency open-to-close return data over short time windows, but such approaches face a trade-off between statistical accuracy and localization. In this paper, I introduce a new estimation framework using high-frequency candlestick data that include open, high, low, and close prices, effectively addressing this trade-off. By exploiting the information contained in candlesticks, the pro- posed method improves estimation accuracy relative to the benchmarks while preserving localization. I further develop a test for spot covariance inference based on candlesticks, which demonstrates reasonable size control and a notable increase in power, particularly in small samples. Motivated by recent work in the finance literature, I test empirically the market neutrality of the iShares Bitcoin Trust ETF (IBIT) using 1-minute candlestick data for the full year of 2024. The results show systematic deviations from market neutral- ity, especially in periods of market stress. An event study around FOMC announcements further illustrates the new method’s ability to detect subtle shifts in response to relatively mild information events.*</span>
<br>

#### <span style="color: #012169;">Working Papers</span>

**Intraday Variation in Systematic Risks and Information Flows**
(with <a href="https://public.econ.duke.edu/~ap172/" class="no-underline">Andrew J. Patton</a>) 
<br> 
<span class="abstract-toggle" onclick="toggleAbstract(this)">Abstract</span> 
<span class="middot">&middot;</span> 
<a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5006587" class="no-underline">SSRN</a> 
<span class="middot">&middot;</span>
<a href="https://www.youtube.com/watch?v=xzrGnCQXz_k" class="no-underline" target="_blank" rel="noopener noreferrer">VTSS Workshop Recording</a>
<span class="abstract-content"> *This paper analyzes variation in the factor structure of asset returns within a trade day by combining non-parametric kernel methods with principal component analysis. We estimate the model on a collection of over 400 high-frequency US equity returns over the period 1996-2020 and show that the proposed model has superior explanatory power relative to a collection of well-known observable factor models and standard PCA. We present a stylized model of asset prices and information flows and show that the factor structure of asset returns varies with the arrival of news. Using data on individual firm earnings announcements, FOMC announcements, and other macroeconomic announcements, we provide evidence consistent with our stylized model, that the superior performance of the proposed model is due to time variation in the factor structure of asset returns around times of information flows.*</span>
<br>

**Generalized Autoregressive Score Trees and Forests**
(with <a href="https://public.econ.duke.edu/~ap172/" class="no-underline">Andrew J. Patton</a>) 
<br> 
*Revised and resubmitted at Journal of Business & Economic Statistics.*
<br>
<span class="abstract-toggle" onclick="toggleAbstract(this)">Abstract</span> <span class="middot">&middot;</span> <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4459756" class="no-underline">SSRN</a> <span class="middot">&middot;</span> <a href="assets/documents/Patton_Simsek_GAS_tree_APPENDIX.pdf" class="no-underline">Online Appendix</a> <span class="abstract-content">  *We propose methods to improve the forecasts from generalized autoregressive score (GAS) models (Creal et. al, 2013; Harvey, 2013) by localizing their parameters using decision trees and random forests. These methods avoid the curse of dimensionality faced by kernel-based approaches, and allow one to draw on information from multiple state variables simultaneously. We apply the new models to four distinct empirical analyses, and in all applications the proposed new methods significantly outperform the baseline GAS model. In our applications to stock return volatility and density prediction, the optimal GAS tree model reveals a leverage effect and a variance risk premium effect. Our study of stock-bond dependence finds evidence of a flight-to-quality effect in the optimal GAS forest forecasts, while our analysis of high-frequency trade durations uncovers a volume-volatility effect.*</span>

#### <span style="color: #012169;">Publications</span>
**Bridging the Covid-19 data and the epidemiological model using the time-varying parameter SIRD model**  
(with <a href="https://sites.google.com/site/cemcakmakli/home" class="no-underline">Cem Cakmakli</a>) 
<br>
*Journal of Econometrics, 242/1, May 2024.*
<br> 
<span class="abstract-toggle" onclick="toggleAbstract(this)">Abstract</span> <span class="middot">&middot;</span> <a href="https://www.sciencedirect.com/science/article/pii/S0304407624001337" class="no-underline">Published Version</a> <span class="abstract-content"> *This paper extends the canonical model of epidemiology, the SIRD model, to allow for time-varying parameters for real-time measurement and prediction of the trajectory of the Covid-19 pandemic. Time variation in model parameters is captured using the score-driven modeling structure designed for the typical daily count data related to the pandemic. The resulting specification permits a flexible yet parsimonious model with a low computational cost. The model is extended to allow for unreported cases using a mixed-frequency setting. Results suggest that these cases’ effects on the parameter estimates might be sizeable. Full sample results show that the flexible framework accurately captures the successive waves of the pandemic. A real-time exercise indicates that the proposed structure delivers timely and precise information on the pandemic’s current stance.*</span>


<!-- #### <span style="color: #012169;">Works in Progress</span>
**Beyond Returns: A Candlestick-Based Approach to Covariance Estimation** *(Draft is coming soon!)*  -->



<script>
function toggleAbstract(element) {
    // Find the next sibling that contains the abstract content
    var abstract = element.closest('span').nextElementSibling;
    while (abstract && !abstract.classList.contains('abstract-content')) {
        abstract = abstract.nextElementSibling;
    }
    if (abstract) {
        abstract.classList.toggle("show");
    }
}

// Add this new function to automatically handle external links and document links
document.addEventListener('DOMContentLoaded', function() {
    // Handle external links (exclude your own domain)
    const externalLinks = document.querySelectorAll('a[href^="http"]');
    externalLinks.forEach(link => {
        // Only open in new tab if it's not your own site
        if (!link.href.includes('yasin-simsek.github.io') && !link.href.includes(window.location.hostname)) {
            link.setAttribute('target', '_blank');
            link.setAttribute('rel', 'noopener noreferrer');
        }
    });
    
    // Handle document links (starting with assets/)
    const documentLinks = document.querySelectorAll('a[href^="assets/"]');
    documentLinks.forEach(link => {
        link.setAttribute('target', '_blank');
        link.setAttribute('rel', 'noopener noreferrer');
    });
});
</script>