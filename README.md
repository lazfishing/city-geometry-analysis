# Evaluating the Geometric Properties of 2D Urban Layouts Using a Data-Driven, Deep Learning Approach

*Why have cities not, long since, been identified, understood and treated as problems of organized complexity? - Jacobs, 1961, p.434.*

Urban planners widely use geometric properties to understand cities, but current methods of quantifying city geometry are very limited. To objectively measure, compare and evaluate urban designs, urban planners need a standard metric to quantify the geometric properties of 2D urban layouts. We use a proprietary tree-structured neural network developed by the AI4CE Lab to encode the complex geometry of urban layouts and learn an expressive representation of city geometry. Using the latent representation of urban layouts, we propose three urban planning applications. Firstly, we classified Manhattan’s urban layouts using GMM clustering algorithms and Shapley interpretations to identify eleven distinct urban layout typologies. Secondly, we derived a standard metric for describing the urban layout composition of neighborhoods using dimensionality reduction. Thirdly, we generated composite urban layouts by decoding the linearly interpolated values of two distinct latent subspaces. These proof-of-concept applications validate our hypothesis that complex city geometry can be encoded using representation learning techniques for downstream urban planning applications.

## Overview

The project uses building footprint data transformed from [RealCity3D](https://ai4ce.github.io/RealCity3D/)'s building polygon dataset. 32 adjacent building footprints were batched as urban layouts for representation learning using a proprietary spatial data auto-encoder developed at AI4CE.

![Project Overview](/images/overview.png)

## Urban Planning Applications

Using the urban layout representations learnt from the auto-encoding process, we propose three urban planning applications.

### Classifyng Urban Layout Typologies

512 latent features are compressed to 50 principal components, explaining 68.8% of the dataset variance. GMM was used to cluster the principal components and classify 11 urban layout typologies, which exhibit distinct layout geometries.

### Measuring Composition of Urban Layout Typologies at Neighborhood Level

By calculating the percentage composition of the 11 urban layout typologies, we are able to define an overall baseline for Manhattan’s urban profile. Similarly, we can calculate the urban profile for each Manhattan Neighborhood Tabulation Area (NTA) to understand their unique patterns.

![Neighborhood Profiles](/images/neighborhood_profiles.png)

We derive a standard metric for measuring the neighborhood urban layout composition by reducing the multi-dimensional neighborhood profile. Using this standard metric, urban planners can evaluate how new urban layouts design change the neighborhood profile, relative to city baselines.

![Spatial Analysis](/images/spatial_analysis.png)

### Generating Composite Urban Layouts

By decoding the linearly interpolated values of two latent subspaces, we are able to generate realistic urban layouts that resemble two dissimilar layouts. Urban planners can use this tool to rapidly generate new layouts that are contextually sensitive to the surrounding urban typology.

![Interpolation Example 1](/images/interpolation.gif) ![Interpolation Example 2](/images/interpolation_2.gif)

## Mentions

This project was completed at the Center for Urban Science and Progress, New York University. The project members Sheung Chan, Lazarus Chok, and Tan Yan Liang.
