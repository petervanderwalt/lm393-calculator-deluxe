# LM393 Universal Comparator Simulator

An interactive web-based tool designed to simplify the process of creating comparator circuits with the popular LM393 IC. This simulator removes the need for complex manual calculations and provides practical, real-world component values for your projects.

**[View the Live Demo Here](https://petervanderwalt.github.io/lm393-calculator-deluxe/)**

## Key Features

*   **Multiple Modes:** Calculate resistor values for various sensor inputs:
    *   **Resistance:** For variable resistance sensors like thermistors or photoresistors (LDRs).
    *   **Voltage:** For sensors that output a direct analog voltage.
    *   **Current:** For circuits that measure current via a shunt resistor.
*   **Optional Hysteresis:** Easily toggle hysteresis on or off.
    *   When **enabled**, it calculates a feedback resistor to create two distinct trip points (an upper and lower threshold), preventing noise-induced chatter around the setpoint.
    *   When **disabled**, it calculates a simple voltage divider for a single, precise trip point.
*   **Practical E96 Resistor Values:** The calculator doesn't just give you ideal resistor values. It finds the closest available **1% E96 standard resistor values**, ensuring your real-world circuit behaves as closely as possible to the simulation.
*   **Dynamic SVG Schematic:** The circuit diagram updates in real-time to reflect your chosen mode and settings. The hysteresis feedback resistor (`Rf`) appears and disappears dynamically, helping you visualize the correct circuit to build.
*   **Interactive Simulation:** A live slider lets you simulate your sensor's input value and instantly see the comparator's output state, complete with a virtual LED and the exact sense voltage being measured.
