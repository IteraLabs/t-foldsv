# tfolds-sv
T Folds Sequential Validation Technique for Financial Machine Learning Models

# Install

pending

# Features

## Folds creation

### Case 1: By Fold Numbers

If the number of folds is provided, then the size for each fold is derived:

1. **Deterministically**
The user provides a fixed number of folds then size for each is calculated in
equal divisions and the last fold might contain residuals.

2. **Probabilistically**
The user provides the probability distribution name, parameters and no. of samples
so to get a known no. of folds then size for each is calculated in 
equal divisions and the last fold might contain residual.

### Case 2: By Fold Sizes

If the fold sizes is provided, then the number of folds is derived:

1. **Deterministically**
The user provides a fixed size to be used for all folds then number of folds is derived
in case of residuals, the last fold might contain residuals.

2. **Probabilistically**
The user provides the probability distribution name, parameters and no. of samples
so to get a known size for the folds, then the total no. of folds is derived.

# Roadmap

## Informational Based Fold Creation

The aim is to provide an information-based criteria to create folds, with a combination 
of either: Fixed number of folds with minimized similarity among all the folds, or, a fixed
range of values [min, max] as a range of accepted similarity between any two folds.

## Embargo space
A purging method to delete data points between folds according to a fixed number of registries.

## Data visualization
Tools and plots for visualizing embargoed spaces, folds creation, information matrix, etc.
