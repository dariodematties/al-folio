---
layout: page
title: nanopore translocations
description: Here I am trying to extract features from noisy signals from nanopore translocations events
img: /assets/img/nt_detection.png
importance: 3
---



This project is a collaboration with the [Department of Electrical Engineering, Solid State Electronics](https://katalog.uu.se/organisation/?orgId=X264:2), [Uppsala University](https://www.uu.se/en).

## Who else is participating?

* [Chenyu Wen](https://katalog.uu.se/profile/?id=N15-1773) and
* [Mauricio Perez](https://katalog.uu.se/profile/?id=N17-1897)


In this project we are using ResNet architectures adapted for one-dimensional data to extract features from noisy signals originated in Nanopore Translocation Events.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/No_Translocation.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Dual_ResNet.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Signal_Features.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
   We use a dual architecture by means of which we predict number of translocation events, average duration and amplitude of all the translocations inside a window in a trace. 
</div>



We are looking forward to detect nanopore tranlocations in noisy signals! To that end we are currently testing Object detection architectures and have obtained some encouraging results.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/nanopore_detection.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Translocation Events Detection in Noisy Signals.
</div>











