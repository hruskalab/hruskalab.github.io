---
layout: page
title: machine learning 
description: correction of chemical property prediction
img: assets/img/redox-ml-approach.PNG
importance: 2
category: work
---
<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/redox-ml-approach.PNG" title="redox steps" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
Redox potentials are a fundamental chemical property, where the accuracy of DFT calculations compared to experiments is limited. To improve the accuracy, I ran both high-throughput explicit solvation similation with [Autosolvate](../3_project), and with machine learning reduced the errors between calculations and experimental data, and analysed the error contributions. 

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/ML-features.PNG" title="ML features" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/solvent-shell.PNG" title="solvent shell convergence" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
For the low number of redox potential data points, machine learning features related to the solute and solvent were used. To optimize the solvent shell size for redox potential calculation, the convergence of redox potential is shown. When combining an explicit solvent shell with implicit solvent (C-PCM) the convergence is reached much faster at around 4 Å. This reduces the computational requirements to calculate redox potentials with an explicit solvent. To optimize the solvent shell size for redox potential calculation, the convergence of redox potential is shown. When combining an explicit solvent shell with implicit solvent (C-PCM) the convergence is reached much faster at around 4 Å. This reduces the computational requirements to calculate redox potentials with an explicit solvent.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/redox-correct.PNG" title="ML correction" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Machine learning could correct both systematic biases and reduce the size of outliers. 
<div class="caption">[Hruska et al. Bridging the experiment-calculation divide: Machine learning corrections to redox potential calculations in implicit and explicit solvent models, 2022]
</div>
[Previous](../3_project)  [Next](../5_project)
