# PCB-Benchmarks

These are PCB benchmarks for automated layout.

Each benchmark is manually placed and routed. Each has a board outline in the Edge.Cuts layer. Each component has one or more courtyard polygons in the F.CrtYd and B.CrtYd layers if applicable.

To use as a layout benchmark, remove the manual routing and ignore the manual placement.

Some components are "locked" as indicated by the locked keyword in their definition. These components must not be moved during automated placement.
