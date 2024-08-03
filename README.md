# parks-pi-server
Parks ADS-B Server configs and helpful information

## General
IP Reservation:  192.168.5.205

## ADS-B Specifc Info 
All Feeders based on the documentation from : <br>
<https://https://sdr-enthusiasts.gitbook.io/ads-b><br>

## ADS-B Ultrafeed Weblinks
<http://adsb.meettheparks.com:8080> : Ultrafeed Home
<http://adsb.meettheparks.com:8080/graphs1090> : Stats & Graphs
<http://adsb.meettheparks.com:8080?pTracks> : Aircraft Tracks
<http://adsb.meettheparks.com:8080?heatmap&realheat> : Heatmap
<http://adsb.meettheparks.com:8080?replay> : Time Lapse


### Ports

|Port|Service|Host|
|---|---|---|
|22|ssh|Native OS|
|1880|Node-Red|Docker|
|1880|MQTT|Docker|
|8080|Ultrafeeder Homepage|Docker|
|8754|FR24 Homepage|Docker|



### Firewall
ufw Enabled
Default Deny Inbound
Default Allow Outbound

Status:  sudo ufw status verbose  
Add Subnet Rule: sudo ufw allow proto tcp from 192.168.0.0/16 to any port 22  
See List of Rules Numbered: sudo ufw status numbered  
Remove Rule: sudo ufw delete 2  

Log Files:  grep -i ufw /var/log/syslog


### System Secrets
All secrets are set as environmental variables <br>

To Set: sudo nano /etc/environment  
To Reload After Saving:  source /etc/environment  