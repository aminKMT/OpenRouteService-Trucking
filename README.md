# OpenRouteService-Trucking
Utilize the OpenRouteService API to estimate the travel time for trucking between the provided origin and destination addresses.

## OpenRouteService API
To utilize these Python scripts for estimating travel time in trucking travel mode, you will need to have an OpenRouteService API. You can obtain the API key and find additional details by visiting https://openrouteservice.org/.
Having the OpenRouteService API key will enable you to leverage the functionalities provided by OpenRouteService for accurate and efficient estimation of travel time for trucking purposes. Ensure that you follow the instructions on the website to acquire the necessary API key and any other relevant information.

## Case and Result
Using these scripts, you can provide the addresses of the origin and destination to estimate the travel time between them, specifically for trucking as the transportation mode. I have already considered an example, where the origin is New York, NY, and the destination is Washington, DC.

```python 
 #Model Inputs:
origin = "New York, NY"  # Replace with your origin address
destination = "Washington, DC"  # Replace with your destination address 
api_key = "Your OpenRouteService API"  # Replace with your OpenRouteService API key

#Utilizing the previously created functions to estimate the travel time for truck travel mode:

travel_time = get_travel_time(origin, destination, api_key)

if travel_time:
    print(f"Estimated travel time between {origin} and {destination} is {travel_time / 60:.2f} minutes.")

else:
    print("Unable to calculate travel time.")
```

### The results can be shown as: 

Estimated travel time between New York, NY and Washington, DC is 371.42 minutes.
