.. title: Physical Modeling: Advanced Models
.. slug: physical-modeling-advanced-models
.. date: 2020-06-10 08:19:59 UTC
.. tags:
.. category: _sound_synthesis:physical
.. link:
.. description:
.. type: text
.. priority: 7



More advanced physical models can be designed,
based on the principles explained in the previous sections.

-----

Resonant Bodies & Coupling
--------------------------

The simple lowpass filter in the example can be replaced by more sophisticated models.
For instruments with multiple strings, coupling between strings can be implemented.


.. figure:: /images/Sound_Synthesis/physical_modeling/plucked-string-instrument.png
	:width: 60%
	:align: center


-----

Scattering Junctions
--------------------

Scattering junctions appear when the acoustic impedance changes,
for example by a change in diameter in a wind instrument.
They can be modeled with allpass filters.
The figure below shows a model of a wind instrument with several waveguides,
connected with scattering junctions (de Bruin, 1995):

.. figure:: /images/Sound_Synthesis/physical_modeling/wind_waveguide.jpg
	:width: 60%
	:align: center


References
==========

.. publication_list:: bibtex/physical_modeling.bib
	   :style: unsrt
