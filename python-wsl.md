## Update WSL
  `sudo apt get update`
  
  OPT: `sudo do-release-upgrade`
  
## Add the Python PPA
  `sudo add-apt-repository ppa:deadsnakes/ppa`
  
## Update and install
  `sudo apt update`
  
  `sudo apt install python3.11-full`
  
## Change the default
  ### Make the old one out (`python3 --version`)
  `sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.10 110`
  
  ### Add the new
  `sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.11 100`
  
  `sudo update-alternatives --config python3`
  
 
 ## Make a venv and activate
  `python3 -m venv . `(/path/to/new/virtual/environment)
  
  `source bin/activate`
  
  
