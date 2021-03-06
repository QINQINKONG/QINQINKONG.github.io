---
layout: post
---


**Kernel density estimation (KDE)** is a nonparametric way to estimate distribution from samples. It can be treated as a substitute of histograms that can give us a smooth and continuous view of the shape of the potential distribution.

When constructing a histogram, we first set up the bin size and count the number of samples falling into each bin which are manifested as the height of the column. In KDE, how we obtain the value of the curve (correpsonding to the height of a column) at a certain location? We achieve this by incorporating a kernel function (such as a normal function) and apply the function value as weights to points surrounding the chosen location (points closer to the chosen locatio will have a higher weights). Then we calculate the weighted sum of all sample points and assign the weighted sum as the final value for this location, and we do the same thing for all locations. This processs is mathematically equivalent to draw a kernal function curve a each sample point and then add all the kernel function curves to form the final distribution curve. 

The bin size in histogram controls how smooth the histogram is. For KDE, the corresponding parameter is bandwidth which does the same thing as bin size for histogram. Basically, a small banwidth means larger weights are given only to the points that are very near to the chosen location.

In practical application, we need to choose the bandwidth and the kernel function, the first of which require some experiments to decide which bandwith is proper. The choice of kernel function seems complicated to me, and it was considered that the Radial Basis Function (RBF) kernel is generally a good choice.

Matthew Conlen has a wonderful post to help people intuitively understand how KDE works [https://mathisonian.github.io/kde/](https://mathisonian.github.io/kde/).
