# BaCon

R code for the Bayesian Connectomics (BaCon) model class, 
developed in "Predicting Phenotypes from Brain Connection Structure"
by Subha Guha, Rex Jung, and David Dunson (2019)

Run "main.R" to 
  (a) Simulate n by p datasets having the same structure as the motivating connectome dataset, MRN-114
  (b) Analyze the data using the BaCon methodology 
  
Before running "main.R" the runtime parameters of function fn.simulation need to be set. These runtime parameters are

  n.burn:     number of burnin MCMC samples
  n.postburn: number of burnin MCMC samples
  num.reps:   required number of independent sets of artifical datasets to be generated and analyzed
  p:          number of predictors (representing brain region pairs as potential predictors)
  n:          number of individuals
  true.r.v:   vector of true concordance parameters, e.g. in Section 4.1 of the paper, true.r.v = c(.875,.925,.975)
  
