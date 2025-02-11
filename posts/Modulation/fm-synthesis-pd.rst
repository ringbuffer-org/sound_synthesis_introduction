.. title: FM Synthesis: Pure Data Example
.. slug: pure-data-fm-example
.. date: 2020-05-11 12:06:11 UTC
.. tags:
.. category: _sound_synthesis:fm-synthesis
.. link:
.. description:
.. type: text
.. has_math: true
.. priority: 7

The following Pure Data example shows a 2-operator FM synthesis with two temporal envelopes.
This allows the generation of sounds with a dynamic spectrum, for example with
a sharp attack and a decrease during the decay, as it is found in many sounds of musical instruments.
The patch is derived from the example given by John Chowning in his early FM synthesis publication:

.. figure:: /images/Sound_Synthesis/modulation/fm-chowning-flow-2.png
	    :width: 400
.. [Fig.1] *Flow chart for dynamic FM with two operators (Chowning, 1973).*


----

The patch `fm_example_adsr.pd <https://raw.githubusercontent.com/anwaldt/sound_synthesis_introduction/main/PD/fm_example_adsr.pd?token=AAJBD23MGOIJCZJB54F2UNTATI2KK>`_ can be downloaded from the repository.
For the temporal envelopes, the patch relies on the abstraction `adsr.pd <https://raw.githubusercontent.com/anwaldt/sound_synthesis_introduction/main/PD/adsr.pd?token=AAJBD233IBWVDKVXQXHOUFDATIZT6>`_, which needs to be saved to the same directory
as the main patch. This ADSR object is a direct copy of the one used in the examples
of the PD help browser.

.. figure:: /images/Sound_Synthesis/modulation/pd-fm-envelope.png
	    :width: 800
.. [Fig.2] *PD FM Patch.*
