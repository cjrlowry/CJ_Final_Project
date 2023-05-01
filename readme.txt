This script is designed to answer research questions on the influence of 
purple sea urchins, Arbacia punctulata, on biofouling and eastern oyster 
quality metrics. The script takes a long-form dataframe, where for each 
bag in the cage (numbered 1-n) the depth, urchin density, mortality, 
biofouling ranking, as well as the set of starting test diameters, ending test 
diameters, ending gonad index percentage (calculation: gonad weight / 
wet weight * 100), and starting/ending shell length. Reference the 
attached example dataset .csv file.

Prior to execution, ensure the example_dataset folder is in your ~/R/ folder.
Other files

The output of this file is an R Markdown file with a series of ANOVA
tests between urchin density and various quality metrics such as GI%,
change in oyster shell length, change in test diameter shell length,
biofouling and urchin mortality. Assumptions such as equivalence of 
variance and correlation of response variables are challenged at the
beginning of the analysis. P-values are printed with significant
values (p <= 0.05) marked with a '*'. Graphs for each test are included 
to visualize the given dataset. A power analysis at alpha = 0.05 and power
= 0.8 was conducted to check a given dataset against and analyze the chance
of Type II error.
