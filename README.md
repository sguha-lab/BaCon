# BaCon

R code for generating simulated data and fitting the Bayesian Connectomics (BaCon) model class,
developed in "Predicting Phenotypes from Brain Connection Structure"
by Subha Guha, Rex Jung, and David Dunson (2019)

Run "main.R". This achieves two aims: 
  (a) Simulates n by p datasets having the same structure as the motivating connectome dataset, MRN-114
  (b) Analyzes the data using the BaCon methodology 
  
Before running "main.R," we need to set the runtime parameters that are passed to function fn.simulation:

  n.burn:     number of burnin MCMC samples 
  
  n.postburn: number of post-burnin MCMC samples
  
  num.reps:   number of independent replications of the simulation, e.g num.reps = 1
  
  p:          number of predictors, representing brain region pairs as potential predictors, e.g. n=50
  
  n:          number of individuals, e.g. n=50
  
  true.r.v:   for each simulation replication, vector of true concordance parameters, e.g. in Section 4.1 of the paper, true.r.v = c(.875,.925,.975)
