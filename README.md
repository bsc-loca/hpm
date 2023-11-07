# Hardware Performance Monitoring counters

This repo contains the RTL of the Hardware Performance Monitoring counters. The module is designed to be used in a RISC-V processor, following the *Zihpm* counter specification*.
Even though the module is separated from the processor, HPM counters are CSR registers. This means that proper interfacing between the CSR module and the HPM module is required.

The module provides 29 generic performance counters, which can be configured by software to count different hardware events.
The [events.md](events.md) file provides the current mapping between the hardware event and its corresponding numerical ID.

**RISC-V specification includes other HPM-related extensions other than Zihpm. Zicntr is implemented inside the CSR module, while other features are work in progress*
