# <p align="center">http-GET//cracked</p>

 <p align="center">
  <img width="560" height="330" src="https://github.com/MBHudson/http-GETcracked/blob/main/main04.png">
</p>


## <p align="center">Automated Mass HTTP-GET Cracker :: Local/Remote(TOR)/Random-Remote(TOR)</p>
### <p align="center">Scans (through the TOR network -to- cleanet) for HTTP-GET services running on a port defined by the user and attempts to crack them with default credentials using Hydra. Capable of scanning (user defined) random or ranged IP addresses at a rate and duration set my the user from the prompts at the beginning of the script, typicaly millions of IPs per minute.</p>

### <p align="center">!ALL SCANNING/CRACKING TRAFFIC IS ROUTED THROUGH THE TOR NETWORK!</p>


<img align="right" width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/pass.jpg">
<img align="right" width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/cam.jpg">



### About:

Once the script is ran you will be given a series of prompts (with examples) asking for the user to define a few parameters; ie: scan duration, scan rate, scan range, port and networking interface (attempts detection but can also be entered by the user). Once the scan is comlete there will first be a "quality control check" attemping to detect any "false positives" the scanner may have picked up. Once this stage is complete the script then moves to attemping to bruteforce the remaining services using hard coded default usernames and passwords. All newly cracked services are shown at the end of the script along with any perviously cracked. All cracked, new and old, are saved under "SAVED_CRACKED" in the script's root directory. Also this script wil save these to an Apache2 server on the user's localhost machine "/var/www/html/cracked.txt" at http://127.0.0.1:80/cracked.txt 

 




### Installation:

Run in a terminal inside root "http-GETcracked" directory:
```shell
sudo chmod +x install && sudo ./install
```


### Usage:
```shell
sudo ./http-GETcracked
```


 <img align="right" width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/banner.jpg"> 
 
### Please Note!

A more recent version of THC-Hydra is required to run this script because of the added "-K" argument. Depending on your current verision you may want to remove your current installation (sudo apt remove hydra) and allow the installer to download the most current version and compile the source code for you. You can also disable this in the installer by commenting out "#" those paricular lines (more details in the installer itself).

<img align="right" width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/router.jpg"> 




### Future:

- [ ] Add "Loop" feature

- [x] ~Add Better documentation with pictures DONE 10/19/22~ 

- [ ] Add better method of defining specific services to be cracked along with specific methods for cracking those services

- [ ] Add user defined username and password lists

- [x] ~Add user defined port: DONE 10/18/22~
