# Dummy-Audio-amplifier
A very basic, 2-stages, audio amplifier, designed with discrete THT components. 
The goal of the project is to build from scratch a simple audio amplifier in order to get familiarity with the main issues of the audio world.

## Main concerns:

- **Noise level**, keep it as low as possible adding decoupling capacitor as close as possible to the LM741 amplifiers (switching noise of the DCDC converter) and using low value resistors (Thermal noise).
- **Limited Bandwidth**, in order to reduce noise r.m.s. and filter out external disturbs.
- **Push-pull final stage thermal runaway**, biasing BJTs with fixed base-emitter voltage cause high dependance on temperature. Introduce emitter resistance to counteract.
- Compensate for Loudspeaker increasing impedance over audio bandwidth with a **Zobel network**.
- Avoid **loop instability** (output stage).
