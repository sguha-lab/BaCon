# BaCon

R code for the Bayesian Connectomics (BaCon) model class, 
developed in "Predicting Phenotypes from Brain Connection Structure"
by Subha Guha, Rex Jung, and David Dunson (2019)

Run "main.R" to 
  (a) Simulate n by p datasets having the same structure as the motivating connectome dataset, MRN-114
  (b) Analyze the data using the BaCon methodology 
  
Before running "main.R," we need to set the runtime parameters that are passed to function fn.simulation:

  n.burn:     number of burnin MCMC samples
  
  n.postburn: number of post-burnin MCMC samples
  
  num.reps:   number of independent replications of the simulation 
  
  p:          number of predictors (representing brain region pairs as potential predictors)
  
  n:          number of individuals
  
  true.r.v:   for each simulation replication, vector of true concordance parameters, e.g. in Section 4.1 of the paper, true.r.v = c(.875,.925,.975)
