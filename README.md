# Adriannaluger.github.io

[![DOI](https://sandbox.zenodo.org/badge/686148950.svg)](https://sandbox.zenodo.org/doi/10.5072/zenodo.10199) 

## Grassland Management Under Climate Change in the Thunder Basin Grassland Region

This project will display a habitat suitability model for Sorghastrum nutans, which are a grass native to North America, that has moved northward in the past 5 decades. The changing of grasslands puts both biodiversity and human well-being in danger, as restoration is very difficult especially if access to native species seeds are unavailable. The model will be based on combining multiple data layers related to soil type, topography, and climate with a focus on the Thunder Basin National Grasslands. The result will show areas with ideal conditions for Sorghastrum nutans to survive in.

## How to run the code

The goal of this project is the end with specific location for where Sorghastrum nutans can be found, or even optimal future locations for it. To begin we must download the Thunder Basin National Grassland boundary so we can confine our other data variables to the area. We then download the soil data and plot both soil and the grassland boundary together. Because the soil data does not cover the entire boundary we must continue this step with multiple tiles, to get all squares next to eachother that are within the boundary. Once we have plotted each tile we can merge them together to get one plot of all the soil data and boundary combined, but before that we must convert the boundary to be the same crs as the soil so then can be plotted in harmony with one another. Next, we download the elevation (srtm) data and plot this along with the boundary as well to see areas of elevation throughout the boundary. Then, we download the climate (precipitation) data, harmonize the longitude, isolate precipitation, and clip/plot the area to show only within the grassland boundary. We then calculate the aspect of the elevation which will be used in the next step to find areas of either ideal or not ideal conditions for Sorghastrum nutans. Similarly, we do this for soil type as well (where ideal conditions are 0-50% sand), and for precipitation (which is ideally 28-114 cm), where the plot shows two colors either being ideal or not accordint to specifc conditions for each raster variable. Then we harmonize all three plots together to ensure they are within the same coordinate systems and will match up correctly. Lastly, we multiple the three together to pinpoint areas that meet ideal conditions for soil type, precipitation, and aspect to create our habitat suitability model for Sorghastrum nutans.


## Usage

This project will be useful to those who are trying to restore grasslands into their natural habitat, to do so though they must find ideal areas for the grasses to thrive in which due to climate change are now different than they used to be. Thus, why it is important to map using a habitat suitability model. 

## License

This project uses the  Apache License, Version 2.0, January 2004. Which can be found at http://www.apache.org/licenses/.

