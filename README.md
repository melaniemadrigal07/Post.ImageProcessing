# Counting Spores + Stacking Images

This repository houses two core scripts:
1. **countspores.R** - Counts spores per image using a fixed grid, then estimates **spores per nL** and **spores per µL**.
3. **stackgray.py** - stacks separate R, G, and B grayscale channel outputs into a single multi-layer grayscale image for downstream processing.


## Requirements
- R (≥ 4.2.0)  
- Packages: `tidyverse`, `igraph`, `vroom`, `ggplot2`

## Inputs
1. **countspores.R**  
   - A folder containing **PNG images** of spores.  
   - The script processes each image, applies filtering and thresholding, then counts spores per grid square.
   - Outputs a .csv file with spore counts of each sample, which can be used for further dilution.
2. **stackgray.py**  
   - A folder with output images from Cytation5 in the R,G,B channels.
   - The script stacks images across the three channels.
   - Outputs folders with stacked images for use in HyPhy.  


       
## Installation
To use this repository, clone it by:
```bash
git clone https://github.com/yourname/HyPhyAnalysis.git
cd HyPhyAnalysis
