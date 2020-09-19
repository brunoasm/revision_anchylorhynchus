# Scripts and data files for revision of **Anchylorhynchus**

This folder includes supplementary scripts and data files used for the revision of Anchylorhynchus, structured in the following folders:

## continuous_traits

Input files used to produce discretized characters in [https://github.com/brunoasm/discretizR](DiscretizR).


## delta

Files for [https://github.com/AtlasOfLivingAustralia/open-delta](delta editor) (*.dlt) and exported directives. 
The delta editor OSX app failed to open in an OSX 10.14.6 (Mojave) with Java Runtime Environment 1.8.0_112. The workaround consisted in opening the jar file directly through the terminal: `java -jar lib/delta-editor-1.02.jar`.

## tnt

Input files and scripts for TNT:
- `anchylorhynchus.tnt` input matrix 
- `find_k.run` TNT macro to test sensitivity to value of k
- `find_k.Rmd` R notebook to visualize results from `find_k.run`
- `search_and_bootstrap.run` modification of the standard `aquickie.run` to search for the best tree and perform symmetric bootstrapping under implied weighting.

## mrbayes

Nexus input file for MrBayes, including matrix and commands.

## phylo_R

Analyses in R, including preparation of figures of phylogenies in the paper and stochastic mapping to infer ancestral states for host association.

- `palm_associations.csv` Table associating species fo Anchylorhynchus with palm genera.
- `anchylorhynchus_chars.tnt` Simplified character matrix to parse in R
- `mrbayes_alphasampled_consensus_rooted.tre` Mrbayes consensus tree, rerooted and saved in Figtree as Nexus
- `tnt_symboot_rooted.tre` TNT best tree, rerooted and saved in Figtree as Nexus
- `Phylo_figure.Rmd` Script to generate figures and do stochastic mapping

## samples_and_maps

R notebooks to produce species distribution maps and lists of specimens studied.

- `create_list.Rmd` R notebook to create a list of specimens studied based on an excel table
- `make_map.Rmd` R notebook to produce the figure with distribution maps in the mais paper.

## supplementary_files

Supplementary files mentioned in the main text: raw data on material studied and raw measurements
