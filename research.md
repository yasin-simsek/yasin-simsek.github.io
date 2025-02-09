---
layout: research
title: "Research"
---

<style>
.abstract-toggle {
    text-decoration: none; /* Removes underline */
    cursor: pointer;
    color: #012169;
}

.abstract-content {
    display: inline-block; /* Makes the abstract visible by default */
    opacity: 1;            /* Ensure it is fully visible */
    transition: none;      /* Removes transition for immediate visibility */
    /* Make abstract hidden by default */
    /* display: none; 
    opacity: 0;
    transition: opacity 0.3s ease-in-out; */
}

.abstract-content.show {
    /* Ensures it appears inline with other elements */
    /* 
    display: inline-block; 
    opacity: 1; 
    */
    /* Hide abstract */
    display: none; 
    opacity: 0;
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


#### Working Papers
* **Intraday Variation in Systematic Risks and Information Flows** 
<br> <span style="font-size: 0.85em;">with <a href="https://public.econ.duke.edu/~ap172/" style="font-size: inherit; text-decoration: none; color: black;">Andrew Patton</a></span> <br> <span class="abstract-toggle" onclick="toggleAbstract(this)">Abstract</span> <span class="middot">&middot;</span> <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5006587" class="no-underline">Draft</a> 
<!-- <span class="middot">&middot;</span> <span style="color:#012169;">Online Appendix</span>  -->
<span class="abstract-content"> *This paper analyzes variation in the factor structure of asset returns within a trade day by combining non-parametric kernel methods with principal component analysis. We estimate the model on a collection of over 400 high frequency US equity returns over the period 1996-2020 and show that the proposed model has superior explanatory power relative to a collection of well-known observable factor models and standard PCA. We present a stylized model of asset prices and information flows and show that the factor structure of asset returns varies with the arrival of news. Using data on individual firm earnings announcements, FOMC announcements, and other macroeconomic announcements, we provide evidence consistent with our stylized model, that the superior performance of the proposed model is due to time variation in the factor structure of asset returns around times of information flows.*</span>

* **Generalized Autoregressive Score Trees and Forests** 
<br> <span style="font-size: 0.85em;">with <a href="https://public.econ.duke.edu/~ap172/" style="font-size: inherit; text-decoration: none; color: black;">Andrew Patton</a></span> <br>
<span class="abstract-toggle" onclick="toggleAbstract(this)">Abstract</span> <span class="middot">&middot;</span> <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4459756" class="no-underline">Draft</a> <span class="middot">&middot;</span> <a href="assets/documents/Patton_Simsek_GAS_tree_APPENDIX.pdf" class="no-underline">Online Appendix</a> <span class="abstract-content">  *We propose methods to improve the forecasts from generalized autoregressive score (GAS) models (Creal et. al, 2013; Harvey, 2013) by localizing their parameters using decision trees and random forests. These methods avoid the curse of dimensionality faced by kernel-based approaches, and allow one to draw on information from multiple state variables simultaneously. We apply the new models to four distinct empirical analyses, and in all applications the proposed new methods significantly outperform the baseline GAS model. In our applications to stock return volatility and density prediction, the optimal GAS tree model reveals a leverage effect and a variance risk premium effect. Our study of stock-bond dependence finds evidence of a flight-to-quality effect in the optimal GAS forest forecasts, while our analysis of high-frequency trade durations uncovers a volume-volatility effect.*</span>

#### Publications
* **Bridging the Covid-19 data and the epidemiological model using the time-varying parameter SIRD model**
<br><span style="font-size: 0.85em;">with <a href="https://sites.google.com/site/cemcakmakli/home" style="font-size: inherit; text-decoration: none; color: black;">Cem Cakmakli</a></span> <br> 
<span class="abstract-toggle" onclick="toggleAbstract(this)">Abstract</span> <span class="middot">&middot;</span> <a href="https://www.sciencedirect.com/science/article/pii/S0304407624001337" class="no-underline">Journal Link</a> <span class="abstract-content"> *This paper extends the canonical model of epidemiology, the SIRD model, to allow for time-varying parameters for real-time measurement and prediction of the trajectory of the Covid-19 pandemic. Time variation in model parameters is captured using the score-driven modeling structure designed for the typical daily count data related to the pandemic. The resulting specification permits a flexible yet parsimonious model with a low computational cost. The model is extended to allow for unreported cases using a mixed-frequency setting. Results suggest that these cases’ effects on the parameter estimates might be sizeable. Full sample results show that the flexible framework accurately captures the successive waves of the pandemic. A real-time exercise indicates that the proposed structure delivers timely and precise information on the pandemic’s current stance*</span>


#### Works in Progress
* **Beyond Returns: A Candlestick-based Approach to Covariance Estimation** *(Draft is coming soon!)* 


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
</script>

<!-- <script>
function toggleAbstract(element) {
    var abstract = element.nextElementSibling.nextElementSibling.nextElementSibling.nextElementSibling.nextElementSibling; // Move to the abstract-content span
    abstract.classList.toggle("show");
}
</script> -->

<!-- <script>
function toggleAbstract(element) {
    var abstractContent = element.nextElementSibling;
    if (abstractContent.style.display === "none") {
        abstractContent.style.display = "inline";
    } else {
        abstractContent.style.display = "none";
    }
}
// document.querySelectorAll('.abstract-toggle').forEach(function(element) {
//     element.style.color = "#012169";
// });
</script> -->

    