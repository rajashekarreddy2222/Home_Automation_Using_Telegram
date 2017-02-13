# home_automation_using_telegram_bots
Author VUYYURU RAJA SHEKAR REDDY 


1.first install rasbian os into raspberry pi

update your os to latest version by following commands
$ sudo apt update /n
$ sudo apt dist-upgrade

Requirements:
C library for Broadcom BCM 2835 as used in Raspberry Pi
This is a C library for Raspberry Pi (RPi). It provides access to GPIO and other IO functions on the Broadcom BCM 2835 chip, as used in the RaspberryPi, allowing access to the GPIO pins on the 26 pin IDE plug on the RPi board so you can control and interface with various external devices.

$ sudo su
$ mkdir project 
$ cd project
$ wget http://www.airspayce.com/mikem/bcm2835/bcm2835-1.50.tar.gz
$ tar -xvzf bcm2835-1.50.tar.gz
$ cd bcm2835-1.50/
$ ./configure
$  make
$  sudo make check
$ make install

 


Installing Nodejs 
$ wget http://node-arm.herokuapp.com/node_latest_armhf.deb 
$ sudo dpkg -i node_latest_armhf.deb

Installing NPM(Node Pakage manager)
$ sudo apt install npm
$ git clone https://github.com/rajashekarreddy2222/home_automation_using_telegram_bots.git
$ cd home_automation_using_telegram_bots
$ npm install node-dht-sensor onoff node-telegram-bot

The available commands are:

 /getouts, shows the actual status of the two relays
 /setout1 ON|OFF, /setout2 ON|OFF, sets one of the outputs to ON or OFF
 /gettemp, shows the actual temperature
 /gethum, shows the actual humidity

Security:

Telegram bots are public, that means that every user can send messages to them.
 To be sure that my bot will answer only to me,
 I added in the code a check on the ID of the user that is sending commands to the bot:
 

 $ sudo node user.js
 $sudo node bot.js
  
  
creating bot in Telegram:
  We can do a lot of stuff with bots. The first step in creating our bot is to talk to the BotFather

  
  Type in the search form BotFather.
  
  Click on the BotFather and a chat container will be opened so we can chat with him. 
  Hit the start button which will display a list of commands that we can use to interact with the BotFather.
 
 Let’s create our bot using the command 
 /newbot 
 It is going to ask for a name for our bot, so we’ll call our bot RajaBot.
 
 Now we have to register for a username, note: it must end in bot, If our bot is named RajaBot the username must be rajabot.
 
 
 
 
 
 
 
 BotFather will congratulate us, and give a link to our bot telegram.me/raja_bot.
 Using one of the commands above, we can make various changes to our bot. 
 But, right now, the most important command is /token, as it will give us an API token to access our bot through HTTPS. Go ahead and type that now:
 
 
 /token
 
 
 
 
 
 The return value will look something like this: 197372558:AAEtvechentOstoPmVyb1_aF2Dbe7k



