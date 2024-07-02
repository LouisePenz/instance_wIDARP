# Instances for the walking and Integrated Dial-A-Ride Problem

The folder instances contains all instances divided in 6 files. For example, for instance with 30 vehicles, 30 requests, number 0:
- `i30_30_0.txt` the file of the instance
- `d30_30_0.txt` the driving time matrix
- `w30_30_0.txt` the walking time matrix
- `public_transport_time.txt` the public transportation time matrix
- `l30_30_0.geojson` locations of the depot, pickups and deliveries
- `stop_locations.geojson` locations of the tramway stops

## Instance file
In the first line, there are:
- number of requests
- number of vehicles
- number of stops
- capacity of vehicles
- time horizon

Each following lines represents a request with:
- id of the pickup
- lower time windows of the pickup
- upper time windows of the pickup
- id of the delivery
- lower time windows of the delivery
- upper time windows of the delivery
- maximum riding time
- quantity of people
- service time

## Time matrix

Let r be the number of requests and s the number of stops. The driving time and walking time matrices have size (1+r+s)*(1+r+s). The depot has index 0, requests go from 1 to r and id of stops go from r+1 to rs.

`public_transport_time.txt` has size s*s.

## Contact

If you have any questions, please send an e-mail to louise.penz@univ-lehavre.fr

