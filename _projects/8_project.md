---
layout: page
title: High-throughput protein simulation
description: open-source software 
img: assets/img/synch-asynch.PNG
importance: 2
category: work
---
Open-source software for complex sampling workflows on 2000+ GPUs
<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/synch-asynch.PNG" title="task allocation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Running adaptive sampling strategies as described [here](../6_project) requires efficient, scalable, and user-friendly execution of both the molecular dynamics and the iterative approach. I led the development of version 2 of the ExTASY software optimized for adaptive sampling. The code is available at <a href="https://github.com/ClementiGroup/ExTASY/">https://github.com/ClementiGroup/ExTASY/</a>. The modular python code allows an user-friendly swap of the molecular dynamics packages or the particular sampling methods with little code change. The Python-based interface to the interoperable and high-performance pilot-based run time system allows the scalability of ExTASY on supercomputers to reach 2000+ concurrent GPUs or concurrent molecular dynamics simulations.  


<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/plot_scalingefficiency.png" title="scaling on supercomputer" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The high scalability of the ExTASY package is enabled by asynchronous execution. The diagram illustrates that in the synchronous case up to 1000s of GPUs have to wait until the analysis step finishes. In contrast, in an asynchronous workflow the GPUs/nodes don't have to wait, significantly increasing the scalability of this heterogeneous use case. 
<div class="caption"> [Hruska et al., Extensible and scalable adaptive sampling on supercomputers., 2020]
</div>
[Previous](../7_project) [Next](../9_project)