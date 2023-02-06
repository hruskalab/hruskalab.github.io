---
layout: page
title: High-throughput explicit solvation
description: open-source software
img: assets/img/autosolvate.PNG
importance: 2
category: work
---

The accurate solvation of molecules with an explicit solvent can be challenging. To make this easier, I codeveloped <a href="https://github.com/Liu-group/AutoSolvate">Autosolvate</a>, an open-source package which allows high-throughput solvation and equilibration of organic systems. In individual steps the systems are generated, pressure-equilibrated, configurationally sampled with QM/MM, and then the clusters of center molecule + solvent shells are extracted. Documentation at <a href="https://autosolvate.readthedocs.io/">https://autosolvate.readthedocs.io/</a>. 


</div>
<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/autosolvate.PNG" title="explicit solvation steps" class="img-fluid rounded z-depth-1" %}
    </div>

</div>

<div class="caption"> [Hruska et al., Autosolvate: A Toolkit for Automating Quantum Chemistry design and Discovery of Solvated Molecules, 2022]

