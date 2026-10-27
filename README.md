# Invisible Forest

**Per-tree Leaf Area Index and shade mapping of the urban canopy from national LiDAR.**

> 🚧 **Release status.** This repository accompanies the manuscript *"Per-Tree Leaf Area Index Mapping Reveals an Invisible Urban Forest and Its Unequal Shade Capacity"* (under review). The full processing pipeline and trained models will be released here **upon publication**. Until then this page is documentation only.

## What this is

A reproducible pipeline that turns a national airborne-LiDAR survey into a **complete, per-tree canopy inventory** for an entire city — deriving leaf area index (LAI), genus-resolved crown transmissivity, and per-tree shade for every tree, not just the ones a municipality has on its books.

It was built on Amsterdam using the Dutch AHN5 survey, and is designed to transfer to any city with comparable national LiDAR (e.g. UK Environment Agency, US 3DEP).

## Pipeline (to be released)

1. **Detect** — individual tree crowns from aerial imagery and LiDAR.
2. **Measure** — per-tree LAI from LiDAR returns via a Beer–Lambert canopy model.
3. **Merge** — match detected crowns against the municipal register to flag registered vs. unregistered trees.
4. **Shade** — per-tree effective shade area from solar geometry and crown transmissivity.

## Data

The derived per-tree dataset is published separately as a Hugging Face dataset:
**[`thrmnn/invisible-forest-amsterdam`](https://huggingface.co/datasets/thrmnn/invisible-forest-amsterdam)** (released upon publication).

## Citation

> Hermann, T. A., van Selm, M., Venverloo, T., Duarte, F., & Ratti, C. (2026). *Per-Tree Leaf Area Index Mapping Reveals an Invisible Urban Forest and Its Unequal Shade Capacity.* (Under review.)

A `CITATION.cff` and the final reference will be added on publication.

## License

Code: to be released under an OSI-approved open-source license (TBD) on publication.
Data: see the dataset card.

## Contact

Théo Alessandro Hermann — `thermann@mit.edu` — MIT Senseable City Lab; AMS Institute.
