# \[Work In Progress\] AMWA BCP-004-02: NMOS Sender Capabilities

[![Lint Status](https://github.com/AMWA-TV/bcp-004-02/workflows/Lint/badge.svg)](https://github.com/AMWA-TV/bcp-004-02/actions?query=workflow%3ALint)
[![Render Status](https://github.com/AMWA-TV/bcp-004-02/workflows/Render/badge.svg)](https://github.com/AMWA-TV/bcp-004-02/actions?query=workflow%3ARender)

<!-- INTRO-START -->

### What does it do?

- Allows an IS-04 Sender to express parametric constraints on the types of streams that it is capable of producing

### Why does it matter?

- Controllers need to know whether a Receiver is capable of handling the streams a Sender is capable of producing before connecting the two
- Controllers need to know whether a Sender is capable of handling specific stream parameters before applying IS-11 active constraints

### How does it work?

- Establishes an open Capabilities register in the NMOS Parameter Registers that lists specifications for parametric constraints (such as width, height, frame rate, number of channels, etc.)
- Defines how a Sender instantiates these Parameter Constraints to make up a list of acceptable Constraint Sets, within the IS-04 `caps` attribute

<!-- INTRO-END -->

## Getting started

There is more information about the NMOS Specifications and their GitHub repos at <https://specs.amwa.tv/nmos>.
