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

**TELEGRAM TOKEN SETUP**
**TELEGRAM SETUP INSTRUCTIONS**
----------------------
 1. Install Telegram and make an account if you haven't already.

 2. Visit https://t.me/botfather and make a bot. (make a note of the API token)
 
 3. Click the provided link to open the chat E.G. "t.me/****bot" then type or click /start)

 4. At the start off the the Script - Replace `$tg` with your Telegram Bot API Token (only when running ps1 directly (not changed using Flipper, VBScript etc as it should be pre-defined there.. eg. `$tg = 'TOKEN'`))
 
 5. Run the script on target system
 
 6. Check telegram chat for 'waiting to connect' message.
 
 7. This script has a feature to wait until you start the session from Telegram.
 
 8. Type the computer name from the 'waiting' message into Telegram bot chat to connect to that computer's session.

*visit https://github.com/beigeworm/Powershell-Tools-and-Toys/tree/main/Command-and-Control for more info*
----------------------------------------------------------------------------------------------------------------------------------------------------

#  If you like my work please leave a star. ⭐

**Notes**

Fast-Execution-Scripts are pulled from github and staged using the 'Invoke-Expession' command.

All other scripts were designed to avoid downloading external scripts or programs.


