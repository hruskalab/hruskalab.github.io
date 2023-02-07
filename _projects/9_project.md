---
layout: page
title: Explainable artificial intelligence
description: ground truth dataset 
img: assets/img/atomwise6.png
importance: 2
category: work
---

Explanations of machine learning can have limited accuracy and reliability. Yet, improvements in explanation approaches are limited by small datasets. We developed a larger dataset with 5 million ground truth explanations for molecular graphs. Chemical validity is guaranteed by using chemical operations, and one explanation value per atom or bond is ensured with decision trees. The resulting pairs of molecules differ only by a change for one atom or bond.

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/atomwise6.png" title="schema atomwise explanation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Explanation values differ for individual elements and ring sizes, but we don't observe a dependency on chemical property values.
<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/fig4-v3.png" title="individual elements" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/pic2-2.png" title="individual elements" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/pic2-3-2.png" title="individual elements" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Similar explanation values for neighboring atoms were observed with topological autocovariance. In contrast to typical synthetic explanation datasets, this dataset can include long-range information.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/pic3.png" title="topological autocovariance" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

This dataset is available on [figshare](https://doi.org/10.6084/m9.figshare.21706829.v1). Crucially; this explanation extraction method can be applied to any existing dataset with molecules and properties. 

<div class="caption"> 
    <a href="https://doi.org/10.26434/chemrxiv-2022-96slq-v2">[Hruska et al., Ground truth explanation dataset for chemical property prediction on molecular graphs, 2022]</a>
</div>
[Previous](../8_project)