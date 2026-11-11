# Inside an HPC cluster

**Live:** https://niznik-dev.github.io/hpc-cluster-tour/

An interactive, single-file tour of what an HPC cluster physically is. You start at a row of racks, then open one rack, then one node, then look at the board inside. Princeton's Della cluster is the running example.

- **Row → rack → node → board:** click down through four levels. Each level has a side panel that explains what you're looking at.
- **Node types:** CPU, large-memory, A100, Grace Hopper, H100 (NVSwitch) and H200 (NVLink bridges), plus login, vis and service nodes.
- **Slurm tie-ins:** each compute node shows how Slurm sees it and the `#SBATCH` lines that request the whole node.

## Accuracy

This is a teaching mash-up, not a floor plan. Compute specs follow Research Computing's public hardware overview. Rack layout, node counts and host names are illustrative, and the board diagrams are simplified schematics. Each level of the page notes where it's guessing.

## Running it

It's one HTML file with no build step and no dependencies beyond Google Fonts. Open `index.html` in a browser, or serve the folder with `python -m http.server`.

To change the hardware, edit the `TYPES` and `RACKSPEC` blocks at the top of the `<script>`.
