# PCB-Benchmarks

These are PCB benchmarks for automated layout as described in DAC 2020 submission 1703.
We have made efforts to anonymize this repo to facilitate the blind academic review process or DAC. The full repo will be updated with author information and so on after the review period.

## Metrics
The primary metrics for PCB layout are through-hole via count, required routing layers, required laser via layers, and area of the smallest rectangular bounding box. These metrics affect manufacturing cost.

A secondary metric is routed track length. It does not affect cost or correctness for these low-speed designs, but may be useful for evaluating the quality of a placement.


## Technical details
Each benchmark is manually placed and routed. 
To use as a layout benchmark, remove the manual routing and ignore the manual placement.

Each design is based on a real design that has been manufactured and tested. The designs in this repo have been modified from the originals to facillitate their use as layout benchmarks.

Each has a board outline in the Edge.Cuts layer. Each component has one or more courtyard polygons in the F.CrtYd and B.CrtYd layers if applicable.

Copper pours ("zones") have been removed from the designs. Nets that used zones for connectivity have been manually rerouted.

The manual routing jobs do not require laser vias; only through-hole vias are used.

Some components are "locked" as indicated by the locked keyword in their definition. These components must not be moved during automated placement.
