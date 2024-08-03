# parks-pi-server
Parks ADS-B Server configs and helpful information

## General
IP Reservation:  192.168.5.205

## ADS-B Specifc Info 
All Feeders based on the documentation from : <br>
<https://https://sdr-enthusiasts.gitbook.io/ads-b><br>

## ADS-B Ultrafeed Weblinks
Ultrafeed Home: <http://adsb.meettheparks.com:8080> <br>
Stats & Graphs: <http://adsb.meettheparks.com:8080/graphs1090> <br>
Aircraft Tracks: <http://adsb.meettheparks.com:8080?pTracks> <br>
Heatmap: <http://adsb.meettheparks.com:8080?heatmap&realheat> <br>
Time Lapse: <http://adsb.meettheparks.com:8080?replay> <br>


### Ports

|Port|Service|Host|
|---|---|---|
|22|ssh|Native OS|
|8080|Ultrafeeder Homepage|Docker|
|8754|FR24 Homepage|Docker|

