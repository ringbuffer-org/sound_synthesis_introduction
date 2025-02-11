.. title: Filters in PD
.. slug: filters-in-puredata
.. date: 2020-06-14 09:00:00 UTC
.. tags:
.. category: _sound_synthesis:subtractive-practical
.. link:
.. description:
.. type: text
.. has_math: true
.. priority: 1


Filters are an essential, sound-defining component within subtractive synthesis.
Especially in analog hardware, filters of specific instruments, like the TB 303 or the Minimoog,
make the individual - almost legendary - sound qualities.
It thus makes sense to look for different filter implementations in software, since they can
improve the overall sound a lot.
PD offers a couple of builtin filters but additional externals come with more elaborate
implementations.

-----


"User-Friendly" Filters
=======================

``lop~``, ``hip~`` and ``bp~`` are the basic non-resonant filters in PD.
The `PD Floss Manuals on filters <http://write.flossmanuals.net/pure-data/filters/>`_ give a nice introduction to
these builtin one-pole filters. The PD help files also come with examples.
Due to the lacking resonance, these filters are not the most interesting ones, musically.
They are also called "user-friendly", since they can not become unstable.


With the example `one-pole-filters.pd <https://github.com/anwaldt/sound_synthesis_introduction/blob/main/PD/one-pole-filters.pd>`_
from the repository, different characteristics of the one-pole filters can be compared, using a band-limited sawtooth as input signal.
Filter cutoff and quality are controlled with control rate signals:

.. figure:: /images/Sound_Synthesis/subtractive/pd-one-pole-filters.png
    :width: 600px
    :figwidth: 100%
    :align: center


-----

Resonant Lowpass Filters
========================

Additional filters can be implemented or installed with Deken.
Filters and the relevant extensions can be found in the `list of external filters <http://write.flossmanuals.net/pure-data/audio-filters/>`_ .
The ``iemlib``, for example,  features many useful resonant filters. One is the 8th order resonant lowpass ``vcf_lp8~``.
The ``moog~`` filter object from the ``flatspace ggee`` library is another good sounding implementation,
trying to emulate the famous Moog Ladder sound.
The example `resonant-lowpass.pd <https://github.com/anwaldt/sound_synthesis_introduction/blob/main/PD/resonant-lowpass.pd>`_
compares the sound of these filters with a square wave input.
For both implementations, all parameters are controlled with audio rate signals.
The slider values are thus converted to signals with the ``line~`` object,
which is basically a linear interpolation.

.. figure:: /images/Sound_Synthesis/subtractive/pd-resonant-lowpass.png
    :width: 600px
    :figwidth: 100%
    :align: center


------

Exercises
=========


.. admonition:: Exercise I

		Control the parameters of the resonant lowpass example with temporal envelopes (ADSR). Use one ADSR for the signal amplitude and one for the cutoff frequency. If the ADSR for the cutoff has a faster decay-release than the one for the amplitude, the sound fill have a sharp onset and a damped release.


.. admonition:: Exercise II

		Trigger the envelope with a metronome sequencer.


.. admonition:: Exercise III

		Create a square wave from the sawtooth and use it as input signal (http://write.flossmanuals.net/pure-data/square-waves/).
