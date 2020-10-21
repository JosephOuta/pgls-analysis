# Pgls analysis

This code depicts a phylogenetic comparative method known as phylogenetic generalized least squares (pgls). The question is: After controlling for phylogenetic history, is there a relationship between eye morphology and activity cycle or trophic level of a mammal? 

The code progression shows: 
line 2-4: reads relevant packages
line 7: reads an array of 100 phylogenetic trees showing possible relationships from a Bayesian inference analysis 
line 8: selects the first tree from the array
line 10: reads trait data containing eye morphology measures and ecological categorical data (activity cycle and trophic level)
line 12: prunes tree data so it matches the available data points on trait data
line 14: attaches trait data to the phylogenetic trees
line 16-40: the analysis - uses pgls function to compute correlation of trait values after controlling for phylogenetic history
line 42-64: the visualizer - uses contMap function to generate a phylogenetic tree diagram showing evolution of the trait 
