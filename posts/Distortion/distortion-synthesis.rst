.. title: Distortion Synthesis
.. slug: distortion-synthesis
.. date: 2020-12-01 13:49:54 UTC
.. tags:
.. category: _sound_synthesis:distortion
.. link:
.. description:
.. type: text
.. has_math: true
.. priority: 1


In contrast to subtractive synthesis, where timbre is controlled by shaping the spectra of waveforms with many spectral components,
**distortion methods shape the sound by adding overtones with different non-linear operations** - like typical distortion.
Waveshaping and wavefolding are the two most common and widely used techniques, useful for creating harmonically rich and dynamically evolving timbres.


-----

Waveshaping
-----------

Waveshaping applies a nonlinear transfer function to a waveform, transforming its harmonic structure. 
The resulting timbre depends on the transfer function and the  amplitude of the input signal.
Waveshaping can **generate controlled harmonic spectra** and is widely used in digital synthesis and computer music.

-----


Early Example: Mutations (Jean-Claude Risset, 1969)
======================================================

When working with early versions of the MUSIC software at *Bell Labs*,
Risset developed **nonlinear synthesis algorithms** to explore continuously morphing spectra.
In *Mutations* this allowed for smooth transitions between timbres and novel synthetic textures.



.. youtube:: u83PZ1NN34s
	:width: 50%
	:align: center



**Quote:**


    “I created spectra that changed their shape in time... A kind of continuous metamorphosis of sound.”
    — Jean-Claude Risset (Roads, 1996)


------


Contemporary Example: Revsic (Richard Devine, 2018)
===================================================

Composed with Eurorack modular synthesizers and multiple Nord G2 Modular units,
Richard Devine's album *Sort\Lave* makes heavy use of waveshaping. 
In *Revsic* this is audible as high-rate modulation of harmonic content,
leading to harsh, metallic textures that evolve in time.
Typical indicators for waveshaping are transitions from smooth waveforms to distorted, clipped shapes.



.. youtube:: NFa2JjPxzdM
	:width: 50%
	:align: center


**Quote:**

    "There are a lot of modular bits in here, where I was using feedback loops and 
    nonlinear processing through analog and digital modules. I was especially interested 
    in wave-shaping and the kind of gritty harmonic transformations that modular synths 
    can provide."  
    — Richard Devine, *Synthtopia Interview*, 2018


------

Notable Instruments
===================



**Doepfer A-136 Distortion/Waveshaper:**

.. figure:: https://www.perfectcircuit.com/media/catalog/product/cache/4d5c1496e5eeb4399ff285086d2de258/d/o/doepfer_a136_01_1.jpg
    :alt: Doepfer A-136 Distortion/Waveshaper
	:width: 15%
    :align: center


- Analog Eurorack waveshaper and distortion module.
- Independent control over positive/negative signal shaping.
- Includes clipping, folding, amplification, and offset sections.



**Mutable Instruments Warps:**

.. figure:: https://pichenettes.github.io/mutable-instruments-documentation/modules/warps/images/manual.png
    :alt: Mutable Instruments Warps
    :width: 20%
    :align: center



- Digital Eurorack module for meta-modulation and waveshaping.
- Multiple shaping modes: diode clipping, wavefolding, rectification, XOR, etc.
- Can interpolate ("morph") between shaping algorithms.








-----


Wavefolding
-----------

Quasi parallel to Bob Moog, **Don Buchla** invented his own system of analog sound synthesis in the 1960s, based on distortion, modulation and additive principles. 
This approach is also entitled **West Coast Synthesis** - in contrast to Moog's *East Coast Synthesis*
Wavefolding is a nonlinear technique where a signal is reflected (or "folded") once it exceeds a certain amplitude threshold. Instead of being clipped, the waveform bends back on itself, creating additional harmonics and a rich, complex spectrum.

Like in waveshaping, the input amplitude controls spectral richness, respectively the strength of overtones.
Wavefolding creates boith harmonic and inharmonic overtones, while 
preserving dynamic responsiveness and musical expressiveness.


-----


Early Example: Silver Apples of the Moon (Morton Subotnick, 1967)
====================================================================

- One of the first electronic compositions using the **Buchla 100** modular system.
- Subotnick exploited wavefolding to generate **organic, evolving tones** that formed a new kind of expressive electronic music.
- No keyboard interface—sound was shaped directly through control voltages and timbre modulation.

    “I was more interested in composing timbre than pitch.”
    — Morton Subotnick (Holmes, 2020)

Subotnick's use of wavefolding anticipated later developments in timbre-driven composition and modular synthesis aesthetics.
The *Buchla 100*   was released in 1965, and was used by Morton Subotnick for his  1967 experimental work *Silver Apples of the Moon*.

.. youtube:: 9HoljsO22qA
	:width: 50%
	:align: center
	

------

Contemporary Example: Tim Hecker
--------------------------------



**Tim Hecker** integrates distortion-based synthesis in his textured, ambient soundworlds. While not always explicitly documented, his use of **modular synthesizers** (e.g., Make Noise, Buchla) suggests significant use of **wavefolding** and related techniques.

**Key Work: *Love Streams* (2016)**

- Employs hardware and software synthesis for **complex harmonic layering**.
- Wavefolding likely contributes to:
  
  - Dense, saturated harmonic fields.
  - Slowly shifting, unstable timbral motion.

- Hecker's practice blends **acoustic processing** with **modular sound design**, pushing beyond traditional electronic genres.

Though not a technical demonstration, Hecker's work showcases how distortion-based synthesis can serve expressive, immersive purposes in contemporary music.

.. youtube:: 8vn9FXebN9g
	:width: 50%
	:align: center



-----

Notable Instruments
===================


**Serge Wave Multipliers:**


.. figure:: https://serge-modular.com/img/euro/Serge_VCM_module_510.jpg
   :alt: Serge Wave Multipliers
   :width: 40%
   :align: center

- One of the earliest analog wavefolder modules (~1974).
- 3 independent processors, including a classic wavefolder.
- Dynamically processes input waveforms to produce new harmonically-related overtones.
- Still produced today (by Random*Source).



**Buchla 259 Complex Waveform Generator**


.. figure:: https://modulargrid.net/img/modcache/2069.f.jpg
   :alt: Buchla 259 Complex Waveform Generator
   :width: 50%
   :align: center

- Contains an internal wavefolder in the “Timbre” circuit
- Paired with sine wave core oscillator to create harmonically rich content
- Voltage-controllable folding amount
- All-analog timbral circuitry to avoid digital aliasing



----

References
----------

- Holmes, T. (2020). *Electronic and Experimental Music: Technology, Music, and Culture*. Routledge.
- Roads, C. (1996). *The Computer Music Tutorial*. MIT Press.
- Synthtopia. (2018, Nov 2). *Richard Devine Interview On Making His New Album Sort\Lave*. Retrieved from https://www.synthtopia.com/content/2018/11/02/richard-devine-interview-on-making-his-new-album-sortlave/
- MOK. (n.d.). *Richard Devine on Waveshaping with Waverazor*. Retrieved from https://www.mok.com/artists.php


