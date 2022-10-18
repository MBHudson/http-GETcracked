# http-GETcracked
##Automated Mass HTTP-GET Cracker:: Local/Remote/Random Remote:: 2022
### http-GETcracked is scanned for HTTP-GET services running on port 80 and attempts to crack them with default password using Hydra. Capable of scanning (user defined) random or ranged IP addresses at a rate and duration set my the user from the prompts at the beginning of the script.

###Usage:
Once the script is run you will give a series of prompts (with examples) asking for the user to define a few paramiters ei: scan duration, scan rate, scan range and networking interface. Once the scan has comleted there first be a "quality control check" attemping to detect "false positives" the scanner may have picked up. Once this stage is complete the script movesonto attemping to bruteforce the remaining services using hard coded default usernames and passwords. All newly cracked services are shown at the end of the script along with any perviously cracked. All cracked, new and old, are saved under "SAVED_CRACKED" in the script's rppt directory. Also this script wil save these on an Apache2 server on the user's localhost machine "/var/www/html/cracked.txt" at http://127.0.0.1:80/cracked.txt

### Installation:
Run in a terminal inside root "http-GETcracked" directory:

sudo chmod +x install
sudo install

### To run the script:

sudo ./http-GETcracked

### Please Note!
A more recent version of THC-Hydra is required to run this script because of the added "-K" option.
Depending on your current verision you may want to remove you current installation and allow the installer to download
the most current version and compile is for you. You can also disable this in the installer by commenting out "#" those paricular lines.
