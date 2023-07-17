# Ducky-Script-For-FlipperZero
A collection of Duckie Scripts which have been updated specifically For badUSB function on the FlipperZero. 
They should however work just fine on any device that uses Ducky Script.
These scripts range from harmless pranks to nefarious red team tools. For educational purposes only! 

**If you want to learn more about the code, most of these scripts are in powershell format here**

https://github.com/beigeworm/Powershell-Tools-and-Toys

# Pre-Deployment Setup
Most of these scripts will require some setup before they will work.
Make sure to read through all the scripts and follow any setup instructions.

**Setup for Telegram, Discord, Dropbox**

**DROPBOX ACCESS TOKEN SETUP**
1. make an app at https://www.dropbox.com/developers/apps (make sure to grant full access to your new app)
2. generate an access token for your app.

**DISCORD WEBHOOK SETUP**
1. (Server Admin Required) On a discord server chat goto > "edit channel" > "integrations" > "webhooks" 
2. make a new webhook, name it and then click "copy webhook URL".

**TELEGRAM BOT SETUP**
1. visit https://t.me/botfather and make a bot.
2. add bot api to script.
3. search for bot in top left box in telegram and start a chat then type /start.
4. add chat ID for the chat bot (use this below to find the chat id) 

`$token='YOUR_TOKEN' #Replace this with your bot Token
$URL='https://api.telegram.org/bot{0}' -f $Token
$inMessage=Invoke-RestMethod -Method Get -Uri ($URL +'/getUpdates') -ErrorAction Stop
$inMessage.result.message | write-output
$inMessage.result.message | get-member`



#  If you like my work please leave a star. ⭐

# Note
all but one of these scripts were designed to avoid downloading external scripts or programs.
