# Competitive classification for complex data

As part of a research project exploring decision-making under uncertainty we gathered a fMRI neuroimaging dataset. We wanted to see if we could identify some neural correlates of strategy exploration in spcific areas of the brain.

This repository includes my initial foray into multivariate MVPA analysis and machine learning.

One of the biggest issues with using ML on fMRI data is how dense and noisy the data is. There aren't really established best practices in this area so we're left to figure it out for ourselves.

To give a sense of how difficult the problem is, a single brain scan includes something like 100,000 individual voxels (3d pixels), each of which is a measure of indirect brain activity. We typically take around 1,000 scans so we have a huge amount of data. The signal we're looking for is typically on the order of less than a 1% change in signal strength.

So each voxel is a "feature" predictor for our ML model. Given the complex nature of the brain, these features interact in high dimensions and so generally speaking there isn't a good linear solution to distinguishing particular behaviors.

# The notebook and data inlcuded here are not the fMRI dataset for privacy concerns.
Instead I provide an example dataset which the script runs on. The basic idea is the same, just that the provided dataset produces much higher accuracy results.
