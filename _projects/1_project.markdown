---
layout: page
title: Language in Cortex
description: In this project I developed neurocomputational theories for the acquisition of language in cortical dynamics
img: /assets/img/EncoderConnections.png
<!--img: /assets/img/12.jpg-->
importance: 2
---

The human brain is the most complex object created by evolution in the known universe.
Yet, how much of this complexity is devoted to exclusively carrying out its algorithmic capabilities
and how much of it has been inherited from biological paths of evolution in order
to work properly in its physical environment?

What if the information processing properties of the brain could be reduced to a few simple
columnar rules replicated throughout the neocortex?

In this research project I seek for those principles by means of the elaboration of computational models
inspired in the neocortex.
On the one hand, the simpler the rules, the more repetitions of such rules are needed in order to get
interesting -human like- behaviours -such as perception invariance.
The mammalian brain -with its possible combinatorial states going beyond the number of atoms in the known universe-
gives us categorical clues in favor of such a position.
On the other hand, the more repetitions of those simple rules, the more computational resources
are needed to implement the models.

I approached this endeavour trying to replicate human early language acquisition capabilities.
I started with human early acquisition of phonotactic rules, specific to a particular language.
I implemented a neurocomputational model whose biological inspiration
-at the cortical level- allowed me to test neurophysiological hypotheses incorporated in the algorithms.
With the desired number of layers, this model abstracted phonological features
in a completely unsupervised fashion.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/EncoderConnections1.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    
Brodmann areas 41 and 42 are parts of the primary auditory cortex. This is the first cortical destination of auditory information stemming from the thalamus. Neural activity in this brain part corresponds most strongly with the objective physical properties of a sound.
Source <a href="https://en.wikipedia.org/wiki/Brodmann_areas_41_and_42" target="_blank">Wikipedia</a>.
Image adapted from <a href="https://svgsilh.com/image/155655.html" target="_blank">here</a> CC0 1.0 Universal (CC0 1.0) Public Domain Dedication.  
Image adapted from <a href="https://doi.org/10.1371/journal.pone.0217966" target="_blank">here</a> under CC-BY licence.
.
</div>



In a posterior work I tested the computational hypotheses previously used for phonetics, but this time, for the acquisition of grammatical features of words inside a sentence context by means of semantic clustering and sequential analysis inside the sentences.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/EncoderConnections.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    
The inferior frontal gyrus has a number of functions including the processing of speech and language in Broca's area. Neural circuitry has been shown to connect different sites of stimulus to other regions of response including other subdivisions and also other frontal gyri..
Source <a href="https://en.wikipedia.org/wiki/Inferior_frontal_gyrus#:~:text=up%20Broca's%20area.-,Function,and%20also%20other%20frontal%20gyri." target="_blank">Wikipedia</a>.
Image adapted from <a href="https://svgsilh.com/image/155655.html" target="_blank">here</a> CC0 1.0 Universal (CC0 1.0) Public Domain Dedication.  
Image adapted from <a href="https://doi.org/10.1371/journal.pone.0217966" target="_blank">here</a> under CC-BY licence.
.
</div>




The algorithms in our hierarchical cortical memory (HCM) are C++14 compliant,
they are composed by a set of classes interrelated by inheritance and composition.
The classes in the algorithms are parallelized by means of OpenMP
-for the classes located at the bottom of the inheritance hierarchy-
and MPI -for the classes at the top of the inheritance hierarchy.
This implementation has the capacity of storing its outputs in Matlab and Octave file formats
and it is suitable for the use of parallel I/O file systems.



This project received High Performance Computing (HPC) mentoring
from [Silvio Rizzi](https://www.alcf.anl.gov/about/people/silvio-rizzi) (HPC assistant at ALCF) and [George K. Thiruvathukal](https://www.luc.edu/cs/people/ftfaculty/gkt.shtml)
(Professor of Computer Science, Loyola University Chicago).
I have been provided with an Argonne Leadership Computing Facility
Allocation whose project name is neurophon and all the code is
allocated in a [GitLab](https://xgitlab.cels.anl.gov/srizzi/neurophon) repository at Argonne.
It is also allocated on [GitHub](https://github.com/neuroph).
By means of Argonne staff assistance, we performed strong and weak
scaling tests in Cooley nodes which returned encouraging results
in terms of multi-threading (OpenMP), multi-processing (MPI) and as an
hybrid implementation (MPI-OpenMP).



<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/inheritance_composition.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Parallelization.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
 Hierarchical Inheritance and Compositional Structure of the Implementation of the models in C++. 
 Towards a High Scalability in Bio-Inspired Models.
 Image adapted from <a href="http://ebooks.iospress.nl/volumearticle/53956" target="_blank">here</a> under CC BY-NC 4.0 licence.
</div>

























