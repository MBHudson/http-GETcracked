# http-GETcracked :: 2022
 <p align="center">
  <img width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/main.jpg">
</p>


##Automated Mass HTTP-GET Cracker :: Local/Remote(TOR)/Random-Remote(TOR) :: 2022
### Scans (through the TOR network -to- cleanet) for HTTP-GET services running on a port defined by the user and attempts to crack them with default credentials using Hydra. Capable of scanning (user defined) random or ranged IP addresses at a rate and duration set my the user from the prompts at the beginning of the script, typicaly millions of IPs per minute.

### ALL SCANNING/CRACKING TRAFFIC IS ROUTED THROUGH THE TOR NETWORK

 <p align="center">
  <img width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/pass.jpg">
</p>


### Usage:

Once the script is ran you will be given a series of prompts (with examples) asking for the user to define a few parameters; ei: scan duration, scan rate, scan range, port and networking interface (attempts detection but can be also be entered by the user). Once the scan is comlete there will first be a "quality control check" attemping to detect "false positives" the scanner may have picked up. Once this stage is complete the script then moves to attemping to bruteforce the remaining services using hard coded default usernames and passwords. All newly cracked services are shown at the end of the script along with any perviously cracked. All cracked, new and old, are saved under "SAVED_CRACKED" in the script's root directory. Also this script wil save these to an Apache2 server on the user's localhost machine "/var/www/html/cracked.txt" at http://127.0.0.1:80/cracked.txt 
 
 <img align="left" width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/cam.jpg"> <img align="right" width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/router.jpg">


### Installation:

Run in a terminal inside root "http-GETcracked" directory:

sudo chmod +x install && sudo ./install


### To run the script:

sudo ./http-GETcracked


### Please Note!

A more recent version of THC-Hydra is required to run this script because of the added "-K" argument. Depending on your current verision you may want to remove your current installation (sudo apt remove hydra) and allow the installer to download the most current version and compile the source code for you. You can also disable this in the installer by commenting out "#" those paricular lines (more details in the installer itself).


 <p align="center">
  <img width="460" height="300" src="https://github.com/MBHudson/http-GETcracked/blob/main/banner.jpg">
</p>

### To Come:

Add "Loop" feature

Add Better documentation with pictures and demo video

Add better method of defining specific services to be cracked along with specific methods for cracking those services

Add user defined username and password lists

~Add user defined port: DONE 10/18/22~
