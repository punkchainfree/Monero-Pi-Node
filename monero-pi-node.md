# How to build - Monero node
**Project - Privacy is key - project 0.1**

Personal Monero Node running on the Raspberry Pi 3 rev. More on my [https://www.patreon.com/punkchain](https://www.patreon.com/punkchain)

Hi! This video is created on livestream at [**twitch.tv/punkchain**](https://twitch.tv/punkchain) (testing, building, scripting are here. etc.. )

**Project description :**
The primary goal was to write monero installation script. Building from source-code for Raspberry Pi 3. (according to monero [Source](https://github.com/monero-project/monero) instruction)

Script was created as training and for support creative community.
 Join, watch or give me feedback #feedback.p0.1
 
**How to** create own **personal monero-node** with cheep hardware **Raspberry Pi 3.**  _Skills and education with results._

**Outputs are**
-  install script `monero-pi-node.sh`
- dd image disc `monero-pi-node.iso` (16GB)
- docs `monero-pi-node.md`

**Hardware**
 - Raspberry Pi 3 - model B
 - MicroSD card or SDD disc with USB-Sata reduction
 - Power supply min. 5V/2A or 5V/3A 
 
 **Software**
 - monero-pi-node.sh - First for [Patrons](https://www.patreon.com/punkchain) at Patreon
 - Putty or bash (SSH)
 - MicroSD card with [pre-installed](https://www.raspberrypi.org/documentation/installation/installing-images/) Raspbian Stretch Lite
 
If you want to learn more about this project, you can support us at Patreon, or watch on Twitch.  **Script** will be released by opensource on [github.com/punkchainfree ](https://github.com/punkchainfree) after 3-6 months [**check it**](https://github.com/punkchainfree).   

**Let's go  to do  - (off stream)**
Run Raspberry Pi with Raspbian

 1. Plug-in MicroSD to Rasp. Pi and connect power supply. 
 2. Plug-in LCD-HDMI and comp. keyboard
 3. Log-in user: **pi**  password: **raspberry** # default user
 4. Enable ssh - by raspi-config utility  
 	Enter `sudo raspi-config` in a terminal window  
 	Select `Interfacing Options`  
 	Navigate to and select `SSH`  
 	Choose `Yes`  
 	Select `Ok`  
 	Choose `Finish`  
 
 5. Find your IP address  
 Enter `ipconfig eth0`  
 Find your IP `inet` 192.168.***.*** according your LAN   
 6.  Check connection to ssh another from other computer  
 Open terminal `ssh pi@ipaddress ` or use putty on M$  
 7. Download [monero-pi-node.sh](https://www.patreon.com/punkchain) script  
 or [github.com/punkchainfree](https://github.com/punkchainfree)  after few months.  
 
**Let's go install it  - (On stream)**
Download  [monero-pi-node.sh](https://www.patreon.com/punkchain) script from Patreon or Github later..

Copy `monero-pi-node.sh` by ssh to raspberry (Linux)  

 1. Open terminal or console ubuntu shortcut `ctrl + alt + t`  
 
 2. Go to _Download directory_ and Copy file via scp or putty   
 $ `cd Downloads`  
 $ `scp monero-pi-node.sh IPADDRESS:/pi/`  
 3. Connect to Raspberry via ssh   
 $ `ssh pi@IPADDRESS` enter default password: _raspberry_  
 4. Add permission and execute flag  
 $ `sudo chmod a+x monero-pi-node.sh`  
 5. Run install script  
 $ `sudo bash monero-pi-node.sh` and enter password  
 6. Bring the coffee ⛾ or something like that will  take about ~2 hours  

	**Waiting to finish installation or compilation.**
 
 8. Test  run monero node ./monerod  
`./monerod`  
 
	**Thank you for being great ✔**
## Some useful command

Help
$ `./monerod --help`  

Run as a daemon in background  
$ `monerod --detach` # run as a daemon in background  
$ `tail -f ~/.bitmonero/bitmonero.log` # watch the logs  
$ `./monerod exit` # ask daemon to exit gracefully  

more in Monero [docs](https://monerodocs.org/interacting/monerod-reference/)  
# Files  
`monero-pi-node.sh` - Patrons first Github later  
`monero-pi-node.iso` (16GB) - Patrons Only  
`monero-pi-node.md` - Patrons first Github later  

## Develop - road map 

Implementation new functions - For example: Integrate support new hardware or port to another OS etc...

|           What     |Date                          |    Finish                     |
|-------------------|-------------------------------|-----------------------------|
| Script - Install script|1st/QR/2019|Done|
| Script - Debuging|1st/QR/2019|?|
| Create - ISO image|1st/QR/2019|?|
| Script - HW Detection RSPI 2,3 |2st/QR/2019|?|
| ISO - Firewall|2st/QR/2019 |?|
| Vote what next|3st/QR/2019 |?|
| Script - upload to github|4st/QR/2019 |?|

`*` - some content is only for patrons and their support
