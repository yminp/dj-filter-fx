# dj-filter-fx
A voltage-controlled DJ filter unit with LFO-like envelope function

## Disclaimer
This design has not yet been validated with a physical prototype. The schematic has been reviewed and analyzed, but practical issues may still be discovered during assembly and testing. A prototype is planned to be built and tested soon.

Anyone building the current revision should treat it as an experimental, pre-prototype design rather than a fully validated production circuit.


## Description
This project is a standalone analog filter effects unit intended primarily for DJ use.

The motivation came from the relative lack of dedicated standalone filter FX units for DJs. Filter effects are built into most modern DJ mixers, but older analog mixers may not provide an integrated filter effect. In those cases, applying a filter generally requires an external effects processor connected through the mixer's send/return path. The goal of this project is therefore to provide a dedicated external filter effect that can be used with such mixers while retaining an analog signal path.

Another major purpose of the project was educational. I wanted to explore the use of operational transconductance amplifiers (OTAs), particularly the LM13700, as voltage-controlled amplifiers (VCAs). In this design, VCAs are used inside a state-variable filter to provide voltage control of both the filter's center frequency and resonance Q. This required treating the OTA not merely as a conventional variable-resistance element, but as a controllable transconductance stage whose gain can be incorporated into the state-variable filter equations.

The project consequently combines several topics that I wanted to study in a practical audio circuit:

- voltage-controlled state-variable filters;
- LM13700 OTA/VCA design;
- voltage control of cutoff frequency and resonance;
- envelope-controlled filtering;
- LFO-based filter modulation;
- analog switching and filter-mode selection;
- balanced audio input and output interfacing;
- gain structure and headroom for professional/DJ audio levels (accepting input up to +26dBu, balanced).

The design is intended both as a usable DJ effects unit and as an experimental platform for learning analog filter and voltage-controlled amplifier design.
