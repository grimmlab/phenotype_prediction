# Comparison Phenotype Prediction

In this repository, we included all simulated phenotypes, precomputed permutation-based GWAS results as well as the 
code for conducting the simulations and generate all figures related to the below-mentioned publication.
In this work, we show a systematic comparison of eight phenotype prediction models. For that purpose,
we used both a variety of synthetic as well as real-world data. All prediction models were optimized using [easyPheno](https://github.com/grimmlab/easyPheno).

## Simulations
We generated synthetic phenotypes using the code in the Jupyter notebook `Simulations.ipynb`. 
The genotype matrix consisting of 10k markers we used for the simulations can be found in the folder `Simulations`. 
Further, all configurations of our simulations including the SNP ids for the causal SNPs and background SNPs as well as their effect sizes can be found in the `Simulations` folder.
We additionally included an overview of the prediction results on all simulated scenarios in `Results`.

## Real-world data
We performed GWAS for four phenotypes of *Arabidopsis thaliana* using [permGWAS](https://github.com/grimmlab/permGWAS). 
The GWAS results can be found in the `GWAS_results` folder. An overview of the prediction results on *Arabidopsis thaliana* can be found in `Results`.

## Results hyperparameter optimization
We further included a detailed overview of the hyperparameter optimzation for each prediction model and phenotype, both for simulated and real-world data, in a .zip-archive in `Results`. There is a .xlsx-file for each phenotype which has different sheets. One sheet gives an overview on the results. Further, there is one sheet for each prediction model with the results per outerfold. Beyond that, there is a sheet with the runtime overview and tried hyperparameter combination for each outerfold and prediction model.

## Plots
The Jupyter notebook `Plot_Scripts.ipynb` contains the code to generate all plots that were shown in the publication and 
to reproduce all analysis regarding feature importance.

## Citation
When using parts of this repository, please cite our publication:

**A comparison of classical and machine learning-based phenotype prediction methods on simulated data and three plant species**  
Maura John, Florian Haselbeck, Rupashree Dass, Christoph Malisi, Patrizia Ricca, Christian Dreischer, Sebastian J. Schultheiss and Dominik G. Grimm  
*under review*

Keywords: Phenotype Prediction, Genomic Selection, Plant Phenotyping, Machine Learning, *Arabidopsis thaliana*.
