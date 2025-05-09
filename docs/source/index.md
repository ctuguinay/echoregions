# Echoregions

Echoregions is a Python Package that interfaces with annotations of water column sonar data for training machine learning models or doing other downstream processing such as biomass estimation.

The annotations are typically regions indicating the presence of specific animal species or lines delineating ocean boundaries, such as the seafloor or sea surface, in the "echogram" (sonar images formed by echo returns). The interfacing functionalities operate in two directions:
- Annotation to ML: Parsing and organizing annotations for preparing training and test datasets for ML developments
- ML to Annotation: Generating annotations from ML predictions that can be used for further downstream processing

At present, functionalities in the Annotation to ML direction have been built for interfacing manual annotations from the [Echoview](https://echoview.com/products-and-services/echoview/) software, which is widely used in the fisheries acoustics community. We plan to add functionalities in the ML to Annotation direction in the near future.

## Functionalities

As of now, Echoregions contains functions to:
- Read, organize, and store Echoview manual annotations (regions and lines)
- Create masks by combining the manual annotations and xarray water column sonar datasets generated by [Echopype](https://github.com/OSOceanAcoustics/echopype)

Note that in Echoregions, the underlying annotation data is stored as a Pandas dataframe, which allows users to directly leverage the powerful indexing and computing functionalities provided by Pandas.

## Contributors

Echoregions development is currently led by Caesar Tuguinay([@ctuguinay](https://github.com/ctuguinay)), with inputs from Wu-Jung Lee ([@leewujung](https://github.com/leewujung)) and Valentina Staneva ([@valentina-s](https://github.com/valentina-s)). Kavin Nguyen ([@ngkavin](https://github.com/ngkavin)) contributed significantly to the initial version.

## Acknowledgement

We thank the NOAA Northwest Fisheries Science Center (NWFSC) Fisheries Engineering and Acoustics Team (FEAT) for supporting this project.

```{image} images/noaa_fisheries_logo.png
:alt: NOAA_fisheries_logo
:width: 200px
```
<!-- <img src="docs/source/images/noaa_fisheries_logo.png" alt="NOAA_fisheries_logo" width="200"> -->

## License

Echoregions is licensed under the open source [Apache 2.0 license](https://opensource.org/licenses/Apache-2.0).

---------------

Copyright (c) 2021-2025, Echoregions Developers.
