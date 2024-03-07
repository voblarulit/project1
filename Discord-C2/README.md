# PoshCord-C2

MAIN SCRIPT HERE - https://github.com/beigeworm/PoshCord-C2

**SYNOPSIS**

Using a Discord webhook and a hosted text file to Act as a Command and Control Platform.

**INFORMATION**

This script will wait until it notices a change in the contents of a text file hosted online (eg. github/pastebin).
Every 10 seconds it will check a file for a change in the file contents and interpret it as a custom command / module.

*Using github to host your command file will take up to 5 minutes to run each module command - Use pastebin (account needed) OR your own server to host the txt file for instant response* 

**SETUP**
1. make a discord bot at https://discord.com/developers/applications/
2. add the bot to your discord server
3. create a webhook in the desired channel on your server. ( channel-settings/integrations )
4. FLIPPER ONLY - goto https://t.ly and make a short link for the webhook. (run prompt only allows 256 characters!)
5. Change WEBHOOK_URL below to your short webhook URL eg. https://t.ly/byuf4e
6. Change BOT_TOKEN below with your bot token
7. Change CHANNEL_ID below to the channel id of your webhook.

**USAGE**
1. Setup the script
2. Run the script on a target.
3. Check discord for 'waiting to connect..' message.
4. Edit the contents of your hosted file to contain 'options' to get a list of modules
5. Do the same with any other command listed - To run that module.

**MODULES**
1. `Message` : Send a message window to the Users desktop.
2. `SpeechToText`  : Send microphone audio transcript to Discord       
3. `Screenshot`  : Sends a screenshot of the desktop to Discord.      
4. `KeyCapture`   : Capture Keystrokes and send to Discord. (see ExtraInfo for usage.)          
5. `Exfiltrate` : Send various files to Discord zipped in 25mb files. (see ExtraInfo for usage.)                   
6. `Upload` : Upload a file to Discord. (see ExtraInfo for usage.)     
7. `Systeminfo` : Send System information as text file to Discord. (takes a few minutes to gather data)
8. `RecordAudio`  : Record microphone to Discord (RecordAudio -t 100) in seconds
9. `RecordScreen`  : Record Screen to Discord (RecordScreen -t 100) in seconds
10. `TakePicture` : Send a webcam picture to Discord. (can take a few minutes..)
11. `FolderTree` : Save folder trees to file and send to Discord.
12. `FakeUpdate` : Spoof windows update screen.
13. `Nearby-Wifi` : Show nearby wifi networks
14. `Send-Hydra` : Never ending popups (use killswitch)            
15. `AddPersistance` : Add this script to the startup folder.         
16. `RemovePersistance` : Remove this script from the startup folder.               
17. `IsAdmin`  : Check if the session is admin.             
18. `AttemptElevate` : Attempt to restart script as admin. (displays a UAC prompt to User)  
19. `EnumerateLAN`  : Show all devices on the network (see ExtraInfo for usage.) (can take a few miniutes to complete)    
20. `Close`  : Close this Session                          
21. `Options`  : Show the Module menu
22. `ExtraInfo`  : Show extra Module information


**FEATURES**

**Custom Scripting**

Edit the hosted file contents to any custom powershell script or command to run custom powershell.

**Killswitch**

Save a hosted file contents as 'kill' to stop 'KeyCapture' or 'Exfiltrate' command and return to waiting for commands.
