# HIF (Hardware Interchange Format)

!!! warning
    HIF is under active development. The documentation is a work in progress and
    may contain errors or incomplete information.

**HIF Project**  is a modular framework for modeling, transforming, and
verifying heterogeneous HW/SW systems, based on the Hardware Interchange Format
(HIF).

---

## Overview

The **HIF Project** is a tightly integrated set of tools and APIs designed to
support modeling, transformation, and verification of heterogeneous HW/SW
systems. At its core lies the HIF format, a unified internal language that acts
as a bridge between various Hardware Description Languages (HDLs) such as VHDL,
Verilog, and SystemC (both RTL and TLM levels).

HIF addresses key pain points in modern hardware design by providing:

- Bidirectional conversion between HDL and HIF
- Seamless integration of components modeled in different HDLs
- Automation for code abstraction, refinement, and fault injection
- A single environment for transactor generation, mutation analysis, and EFSM extraction

By offering a standardized internal format and robust manipulation APIs, HIF
enables faster design reuse, improves simulation performance, and supports
safety-critical verification processes that would otherwise require multiple
disconnected tools.

---

## Key Features

- Bidirectional HDL to/from HIF conversion
- Integration of heterogeneous HDL components
- Abstraction and refinement of HDL models
- Fault injection and post-refinement verification
- Extensible APIs for advanced code manipulation
- Support for both front-end and back-end transformation tools

---

## Repositories

HIFSuite is organized into three main repositories:

- **[hif-core](https://github.com/esd-univr/hif-core)**
  Contains the HIF abstract syntax tree (AST) representation and the core
  functionality for visiting, analysis, and manipulation of HDL models.

- **[hif-frontend](https://github.com/esd-univr/hif-frontend)**
  Provides front-end tools to convert existing HDL code to HIF.
  Current tools include:
      - `verilog2hif`: Verilog to HIF converter
      - `vhdl2hif`: VHDL to HIF converter

- **[hif-backend](https://github.com/esd-univr/hif-backend)**
  Implements back-end tools to generate HDL code from HIF.
  Current tools include:
      - `hif2sc`: Generates SystemC code from HIF
      - `hif2verilog`: Generates Verilog code (currently incomplete)

---

## Publications

- **`HIFsuite: tools for HDL code conversion and manipulation.`** Nicola Bombieri,
Giuseppe Di Guglielmo, Michele Ferrari, Franco Fummi, Graziano Pravadelli,
Francesco Stefanni, and Alessandro Venturelli. EURASIP J. Embedded Syst. 2010,
Article 4 (January 2010), 20 pages.
**[https://doi.org/10.1155/2010/436328](https://doi.org/10.1155/2010/436328)**

---

## License

HIF is released under the BSD 2-Clause License.

---

## Contact

For technical support, collaborations, or further information, contact:

Enrico Fraccaroli (<enrico.fraccaroli@univr.it>), Department of Engineering for
Innovation Medicine University of Verona, Italy
