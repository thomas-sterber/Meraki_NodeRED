Step by Step instructions on how to install Node-RED on MAC , Raspberry or Debian
and use the Meraki PlugIn

# Node-RED on MAC

## Install brew
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

## Install npm
  brew install npm

## Install last stable Node.js
  sudo npm cache clean -f
  sudo npm install -g n
  sudo n stable


## Install Node-RED
  sudo npm install -g --unsafe-perm node-red

## start stop Node-RED
  start :        #node-red
  open Browser:  http://localhost:1880
  stop :         Ctrl+C 



# Node-RED on Raspberry



# Node-RED on Debian



# Node-RED Palette's

## Meraki
  Manage Palette > Installs > search meraki , install
  https://github.com/dexterlabora/node-red-contrib-meraki-dashboard-api
  cd ~/.node-red
  npm install git+https://github.com/dexterlabora/node-red-contrib-meraki-dashboard-api

## Dashboard


# Node-RED Links
  getting_started
  Meraki_Node-RED_101    https://developer.cisco.com/docs/meraki-dashboard-api-node-red-node/







