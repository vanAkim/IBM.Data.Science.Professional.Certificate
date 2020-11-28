# Synopsis

## Problematic

Toulouse is the fourth largest city in France and although it remains relatively human sized, like most European cities apart from the capitals, there is a strong socio-economic activity. Several reasons could explain it, it is among others the European capital of the aeronautical and space industry, and a city with many universities. There is therefore a strong mixing of the population and a significant dynamism within the city.

Like many other cities in the world, especially with a large population of students and young workers, some neighborhoods are well-known to have many bars. Since I live there, I have at least 3 places in mind with a very high density of bars in small spaces (i.e. ~ 10/20 next to each other). It would be interesting to have a more in-depth look at this phenomenon, however the issue referred into this report concerns clustering but not with regard to bars (in the same way as streets containing only shops). The theme is the one of culture and related places for the public.

Since there are clusters of bars, are there geographic groupings of cultural points?
And if so, are these cultural places more or less grouped according to their category?

This summary analysis could be an entry point for the City of Toulouse to know the extent of its cultural area. In addition, with related data and analyzes on these cultural places (e.g. number of visitors over years, proximity to public transports, etc.) it might be possible to know whether it is better to implement a museum away or not from other points of interest. The same conclusion can be drawn for the cultural industry, does one cinema close to another attract more or less spectators?

This report does not have as much ambition and just seeks to present a distribution of cultural places referenced on Foursquare, with a summary analysis on their geographical distribution and with respect to their category.

## Data used

### 1. Cultural venues

The main points, i.e. cultural places, will be retrieved from Foursquare databases using their API. However, Foursquare's data is relatively biased since among all the cultural places in Toulouse (it is possible, for example, to find lots of these locations in different data sets on [Data.toulouse-metropole](https://data.toulouse-metropole.fr/explore/?refine.theme=Culture&sort=modified) website) a very small fraction is identified. This may be the result that the Foursquare service is little used by the resident or tourist population in this city or in France, or that the way Foursquare generates its points of interest, or that cultural places visitors are rarely inclined to list their experiences on Foursquare. Nevertheless, it is possible in a way to take advantage of this bias without too much impacting the initial problematic. 

Indeed, since the places of Foursquare are brought and developed by the users on the spot, the sites listed are probably those which attract the most attention. So, under the assumption that Foursquare places are the most attractive ones in the city, then the above questions are still relevant when looking only at the main cultural places.

### 2. Pedestrian count

On [Data.toulouse-metropole](https://data.toulouse-metropole.fr/explore/dataset/comptages-pietons/information/?sort=annee&location=16,43.60208,1.44634&basemap=jawg.streets) webpage a dataset is available which counts the pedestrian flows in different streets of Toulouse. This `comptages-pietons` dataset, from **Toulouse Métropole**, with last data input on **2020-02-13**, is made available under the [Open Database License](http://opendatacommons.org/licenses/odbl/1.0/) ([local license text](https://github.com/vanAkim/IBM_Data_Science_Professional_Certificate/blob/main/9-Capstone_Project/FinalProject/ODC%20Open%20Database%20License%20(ODbL).md)). Any rights in individual contents of the database are licensed under the [Database Contents License](http://opendatacommons.org/licenses/dbcl/1.0/).  

Data could help better to cluster the cultural venues. In addition, another question that could have been added to the problematic is whether there is a correlation between the geographical position and the category of cultural places with the number of pedestrians in nearby streets. It's easy to think that the position of a historical monument or museum is determined by its long history and not by the flow of pedestrians of recent years. Conversely, a mainstream cinema probably preferred to set up in a busy street.

Unfortunately, the measurement methodology is slightly insufficient to have the most enlightened information. Indeed, only a few streets of the city were targeted, within a very short timeframes (~1h/day), and just one day a year. Also, some pedestrians can be counted several times in succession or on the contrary some others never counted. The advantage of this method lies in the estimation of pedestrian traffic and its evolution. That's why none related question was added to the problematic section, this dataset is mostly a bonus exploratory analysis with a potential relevant result.

## WORK IN PROGRESS - Analysis notebook

The analysis jupyter notebook is named *[Culture venues clustering in Toulouse](https://github.com/vanAkim/IBM_Data_Science_Professional_Certificate/blob/main/9-Capstone_Project/FinalProject/Culture%20venues%20clustering%20in%20Toulouse%20-%20Coursera%20Capstone.ipynb)* and can be viewed with *INCOMING LINK*.
