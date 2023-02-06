---
layout: page
title: Explicit solvation
description: at DFT accuracy
img: assets/img/mddf2.PNG
importance: 2
category: work
---


<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/aspheric.PNG" title="aspheric" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/mddf2.PNG" title="mddf" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The solvation of molecules frequently has a large influence on the molecule. To better understand this influence, accurate models of explicit solvents are necessary. With <a href="https://github.com/Liu-group/AutoSolvate">Autosolvate software,</a> described [here](../3_project), accurate equilibration and sampling of a solvent shell can be reached. To reduce the computational requirements when calculating quantum mechanical properties with this solvent shell, the solvent shell size has to be selected carefully. Spherical solvent shells (top figures) don't cover the molecule as consistently as aspherical solvent shells. 

Solvent shells can be detected with radial distribution functions (RDF), but for comparing solvent shells of molecules with different sizes, an RDF shifted by the average molecule radius can be beneficial (lower figures). For aspherical molecules, which are very common, the minimum distance distribution function (MDDF) shows the solvent shells much clearer than a RDF. MDDFs measure the minimum distance between the molecule and solvent instead of the distance to the center of the molecule. 

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/closeness.PNG" title="closeness" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/closeness-solvent.PNG" title="closeness solvent" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
The MDDF allows one to measure the dependency of the closeness between the molecule and solvent on the molecule. With machine learning this closeness relationship can be predicted from the molecule structure. The closeness depends on the solvent and is decreasing with the solvent's dielectric constant. 

<div class="caption">
    [Hruska et al., Autosolvate: A Toolkit for Automating Quantum Chemistry design and Discovery of Solvated Molecules, 2022]
</div>

