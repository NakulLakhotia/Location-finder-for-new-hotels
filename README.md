# Location-finder-for-new-hotels

### Uses Data Science and Unsupervised Machine Learning (Clustering Algorithm) to find feasible locations for building new hotels

### Data Source - https://en.wikipedia.org/wiki/List_of_cities_in_India_by_population


### Steps involved:

#### 1. Find relevant data

#### 2. Extract Data 
        
        The data was extracted from the wikipedia using Beautiful Soup
        
#### 3.Geographical coordinates of the cities & Mapping with Folium 
        
        3.1 Using the Geocoder package convert the addresses into geographical coordinates in the form of latitude and longitude
        
        3.2 Populate the data into a pandas DataFrame and then visualize the neighbourhoods in a map using Folium package
        
#### 4.Use Foursquare API

        4.1 Create a developer account - [Foursquare Developer](https://developer.foursquare.com/)
        
        4.2 Make API calls to Foursquare passing in the geographical coordinates of the neighbourhoods in a Python loop
        
        4.3 Analyse each neighbourhood by grouping the rows by neighbourhood and taking the mean of the frequency of occurrence of each venue category
        
        4.4 Filter the “Hotel” as venue category for the neighbourhoods
        
#### 5.Clustering

        5.1 Use K-Means to cluster the neighbourhoods into 3 clusters based on their frequency of occurrence for “Hotel”
        
        5.2  The clusters will allow us to identify which neighbourhoods have lower concentration of hotels within a radius of 5km
        
        5.3  Identify which neighbourhoods are most suitable to open new hotels according to their tourism popularity. 
        
#### Note : For better understanding, view the report and the code above 
        
