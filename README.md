## Overview
This repository provides several R scripts enabline to perform numerical simulations for pH kinetics of meat products under different user-defined formulation-atmosphere conditions. These scripts gives possibilities to apply a Bayesian modelling procedure to describe pH changes and estimate acidification rates for experimental data collected on food matrices, with user-defined atmosphere factors and/or formulations (expressed as concentrations). 

## The provided dataset ## 
The dataset corresponding to our study is provided: pH measurement of different meat samples made in different batches ("Lot"), with different formulations ("Lactate"), packed under several modified atmosphere ("Atm"), and measured at different time points ("Time")
The formulation used in our is potassium lactate. The lactate contents, denoted Lactate, is included in the model as a variate. The effect of the different modified atmosphere conditions modelled as multi-level factor (3 levels in our study) are denoted 'deltaAir', 'deltaMAP1', 'deltaMAP2'. For further use of the model, rename these variates in the scripts conveniently as well as in the dataset. 

## To get started
The dataset has to be structured as table with at least the following columns
- SampleCode: the unique id the sample
- Atm: the modified atmosphere
- Lactate (can be renamed in the dataset and in the script if applied for other formulations): lactate concentrations
- Time: sampling time (storage time)
- pH

## Modelling procedure
Check the R script: "acidification_bayesianinference.R"

## Associated article (in submission)
Modelling acidification of fresh meat products in a study framework of spoilage depending on formulations and modified atmosphere: a Bayesian approach.
Authors: Ngoc-Du Martin Luong, Louis Coroller, Monique Zagorec, Nicolas Moriceau, Valérie Anthoine, Sandrine Guillou, Jeanne-Marie Membré
R/git contributor: Ngoc-Du Martin Luong (ngoc-du.luong@anses.fr)
Corresponding author: Jeanne-Marie Membré (jeanne-marie.membre@oniris-nantes.fr)
