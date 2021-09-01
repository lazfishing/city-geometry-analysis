# Evaluating the Geometric Properties of 2D Urban Layouts Using a Data-Driven, Deep Learning Approach

*Why have cities not, long since, been identified, understood and treated as problems of organized complexity? - Jacobs, 1961, p.434.*

Urban planners widely use geometric properties to understand cities, but current methods of quantifying city geometry are very limited. To objectively measure, compare and evaluate urban designs, urban planners need a standard metric to quantify the geometric properties of 2D urban layouts. We use a proprietary tree-structured neural network developed by the AI4CE Lab to encode the complex geometry of urban layouts and learn an expressive representation of city geometry. Using the latent representation of urban layouts, we propose three urban planning applications. Firstly, we classified Manhattan’s urban layouts using GMM clustering algorithms and Shapley interpretations to identify eleven distinct urban layout typologies. Secondly, we derived a standard metric for describing the urban layout composition of neighborhoods using dimensionality reduction. Thirdly, we generated composite urban layouts by decoding the linearly interpolated values of two distinct latent subspaces. These proof-of-concept applications validate our hypothesis that complex city geometry can be encoded using representation learning techniques for downstream urban planning applications.

## Overview

The project uses building footprint data transformed from [RealCity3D](https://ai4ce.github.io/RealCity3D/)'s building polygon dataset. 32 adjacent building footprints were batched as urban layouts for representation learning using a proprietary spatial data auto-encoder developed at AI4CE.

![Project Overview](/images/overview.png)

## Urban Planning Applications



## Mentions

This project was completed at the Center for Urban Science and Progress, New York University. The project members Sheung Chan, Lazarus Chok, and Tan Yan Liang.
