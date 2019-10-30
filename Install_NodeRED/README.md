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
    bash <(curl -sL https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered)
    sudo apt-get install build-essential
    
## start stop Node-RED
    start:           node-red-pi --max-old-space-size=256   (locally in terminal)
    stop :           Ctrl+C     (locally)
    
    start service:   node-red-start     (as a background service)
    restart service: node-red-restart 
    stop:            node-red-stop
    
    open Browser:    http://localhost:1880    or http://<IP>:1880
    
## configure autostart
    sudo systemctl enable nodered.service
    sudo systemctl disable nodered.service
    


# Node-RED nodes

## Install most important nodes
    cd ~/node-red/
    npm install node-red-dashboard
    npm install node-red-node-base64
    npm install node-red-node-random
    npm install node-red-node-ui-table
    npm install node-red-contrib-ui-media

## Install Meraki node

    npm install node-red-contrib-meraki-dashboard-api

NodeRED GUI:
  Manage Palette > Installs > search meraki , install
  (node-red-contrib-meraki-dashboard-api)


## Node-RED Links
[Meraki_Node-RED_101]

[Meraki_NodeRED_Node]

[NodeRED.org]




[Meraki_Node-RED_101]: <https://developer.cisco.com/docs/meraki-dashboard-api-node-red-node/>
[Meraki_NodeRED_Node]: <https://github.com/dexterlabora/node-red-contrib-meraki-dashboard-api>
[NodeRED.org]: <https://nodered.org/docs/getting-started/raspberrypi>

