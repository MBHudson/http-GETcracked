# http-GETcracked :: 2022

##Automated Mass HTTP-GET Cracker :: Local/Remote(TOR)/Random-Remote(TOR) :: 2022
### Scans (through the TOR network -to- cleanet) for HTTP-GET services running on port 80 and attempts to crack them with default password using Hydra. Capable of scanning (user defined) random or ranged IP addresses at a rate and duration set my the user from the prompts at the beginning of the script.


### Usage:

Once the script is run you will give a series of prompts (with examples) asking for the user to define a few paramiters ei: scan duration, scan rate, scan range and networking interface (attempts detection but can be also entered by the user). Once the scan is comleted there will first be a "quality control check" attemping to detect "false positives" the scanner may have picked up. Once this stage is complete the script then moves onto attemping to bruteforce the remaining services using hard coded default usernames and passwords. All newly cracked services are shown at the end of the script along with any perviously cracked. All cracked, new and old, are saved under "SAVED_CRACKED" in the script's root directory. Also this script wil save these to an Apache2 server on the user's localhost machine "/var/www/html/cracked.txt" at http://127.0.0.1:80/cracked.txt 
                                 
### ALL SCANNING/CRACKING TRAFFIC IS ROUTED THROUGH THE TOR NETWORK


### Installation:

Run in a terminal inside root "http-GETcracked" directory:

sudo chmod +x install
sudo install


### To run the script:

sudo ./http-GETcracked


### Please Note!

A more recent version of THC-Hydra is required to run this script because of the added "-K" option. Depending on your current verision you may want to remove your current installation (sudo apt remove hydra) and allow the installer to download the most current version and compile is for you. You can also disable this in the installer by commenting out "#" those paricular lines.


### To Come:
Add "Loop" feature
Add Better documentation with pictures and demo video
Add better method of defining specific services to be cracked along with specific methods for cracking those services
Add user defined username and password lists
