# Shared Evolutionary History Shapes Skeletal Shape in Flatfishes
Black and Berendzen 20##

---

This code completes PCA and ANOVA analyses and generated publication figures.

### Required R packages

`geomorph` , `StereoMorph` , `phytools` , `ape` , `dplyr` , `vegan` , `devtools` , and `ggbiplot`

### Load data
Landmarks are in the form of a TPS file. Use `readland.tps` to load data into R environment.

### Averaged individuals by species
Use `aggregate` to find the average landmark coordinates per species.

### Phylomorphospace
Use `read.tree` to read tree file, and `drop.tip` to remove species from the tree that are not in the landmarked file.
Code will produce figures 3, S4, S5, and S6 (interactive).

### Chronophylomorphospace
Produces figures 4 and S7 (interactive).

### Phylogenetic Signal
Use `physignal` in Geomorph to generate the phylogenetic signal and produces Figure S8.

### Backtransformation Flatfishes
Use `btShapes.R` (https://aaronolsen.github.io/tutorials/morphometrics/backtransform.html) to generate figures 2, and S3.

### Input Ecological Data and Procrusties ANOVA and Pairwise
Generate ANOVA in a phylogenetic context for shape and ecological data using `procD.pgls` and `pairwise`.

### Plot ecological preferences to phylomorphospace
Produces single figure (figure S9) with 4 plots for each significant ecological type.
