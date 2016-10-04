##Introduction

This project concerns the sanitation issues in the area of city of Boston. Five data sets are used to analyze the requests of street cleaning and dead animal pickup, and the numbers of community gardens in certain neighborhoods.
If a neighborhood has a large number of gardens, and requests lots of dead animal pickups, such neighborhood is very likely in need of animal control. 

retrieve.py retrieves five data sets as resource, and produce four data sets, which are subsets of "311, Service Requests" and "Mayors 24 Hour Hotline".
process.py uses the four data sets produced from retrieve.py combined with "Community Gardens" to figure out the numbers of gardens and requests associate with neighborhoods.
neighborhood_locations.py finds geo-locations(longitudes and latitudes) of every neighborhood, to provide the basics of further research.

##To Run

Please use python3 to run following files in order:

retrieve.py

process.py

neighborhood_locations.py

##Authentication

```
{"user": DB_USER,
"service": {
	  	"cityofbostondataportal": {
            "service": "https://data.cityofboston.gov/",
            "username": "USER",
            "password": "PASSWORD",
            "token": "TOKEN",
        }        
}
```
