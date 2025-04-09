.. title: Digital Synthesis: History & Taxonomy
.. slug: synthesis_history_taxonomy
.. date: 2020-04-27 15:00:32 UTC
.. tags:
.. category: _sound_synthesis:introduction_2
.. link:
.. description:
.. type: text



Taxonomy
--------

Digital methods for sound synthesis can be grouped according to their underlying principle of operation.
In 1991, Smith proposed four basic categories:

.. figure:: /images/Sound_Synthesis/synthesis_taxonomy_SMITH.png
  :width: 60%
  :figwidth: 100%
  :align: center
  
  *Taxonomy of synthesis algorithms (Smith, 1991).*



Processed Recording
===================

Already a technique in the analog domain (*Musique Concrète*), 
this family of synthesis approaches makes direct use of previously recorded sound for synthesis.
This can be the playback of complete sounds or the extraction of short segments, such as grains or even 
single periods of a sound (*wavetable*).




Spectral Models
===============

Spectral models analyse and synthesize sounds through mathematical models of their spectra and their development over time.
They are **receiver-based**, since they model the sound as it is perceived by the listener.
As an extension of additive synthesis, spectral models use basic components like **sinewaves and noise** to create musical sounds with high accuracy.


Physical Models
===============

Physical Models are digital emulations of physical processes in musical instruments.
Basic building blocks like oscillators, resonating bodies and acoustic conductors
are realized as buffers and digital filters. 
Physical modeling is regarded a **source-based** approach, since it models the sound generation process.


Abstract Algorithm
==================

If it is not processed sound, a spectral model or a physical model, it is an abstract algorithm.
Algorithms from this category often transfer methods from other domains, like radio technology (FM Synthesis),
to the musical domain.


Neural Networks & Deep Learning
===============================

The above introduced taxonomy is still valid but misses some recent developments. 
Methods based on neural networks and deep learning for sound generation may be considered a fifth taxon.



-----


Family Tree
-----------

The synthesis experiments at Bell Labs are the origin of most methods for digital sound synthesis.
This figure illustrates the relations for a subset of synthesis approaches, starting with Mathews:


.. figure:: /images/Sound_Synthesis/bilbao_history.png
  :width: 60%
  :figwidth: 100%
  :align: center

  *Evolution and family tree (Bilbao, 2009).*


The foundation for many further developments was
laid when John Chowning brought the software MUSIC VI
to Stanford from a visit at Bell Labs (Chowning, 2011).
After migrating it to a *PDP-6* computer,
Chowning worked on his groundbreaking digital compositions,
using the FM method and spatial techniques.


------


.. publication_list:: bibtex/synthesis_overview.bib
	   :style: unsrt
