#-------------------------------------------Nano Max-----------------------------------------------------------
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Welcome to GitHub Desktop!
This is your README. READMEs are where you can communicate what your project is and how to use it.
Write your name on line 6, save it, and then head back to GitHub Desktop.
---------------------------------Server.cfg--Starts-Here-------------------------------------------------------
#   ____  ____   _____               
#  / __ \|  _ \ / ____|              
# | |  | | |_) | |     ___  _ __ ___ 
# | |  | |  _ <| |    / _ \| '__/ _ \
# | |__| | |_) | |___| (_) | | |  __/
#  \___\_\____/ \_____\___/|_|  \___|
## You CAN edit the following:
endpoint_add_tcp "0.0.0.0:30120"
endpoint_add_udp "0.0.0.0:30120"
sv_maxclients 48
set steam_webApiKey "none"
sets tags "default, deployer, qbcore, qb-core"
## You MAY edit the following:
sv_licenseKey "---Your License Key-----"
sv_hostname "Host Name (Name Visible in FiveM)"
sets sv_projectName "Project-Name"
sets sv_projectDesc "Project Descripton(An advanced FiveM RP framework including jobs, gangs, housing & more!)"
# Language
sets locale "en-US" 
# Logo
load_server_icon myLogo.png 
set sv_enforceGameBuild 2372
# Database Link Confuguration
set mysql_connection_string "mysql://root@localhost/QBCoreFramework_4B04D1?charset=utf8mb4" 
# Voice config
setr voice_useNativeAudio true
setr voice_useSendingRangeOnly true
setr voice_defaultCycle "GRAVE"
setr voice_defaultVolume 0.3
setr voice_enableRadioAnim 1
setr voice_syncData 1
# QBCore locale config
setr qb_locale "en"
# QBCore UseTarget
setr UseTarget false
# These resources will start by default.
ensure mapmanager
ensure chat
ensure spawnmanager
ensure sessionmanager
ensure basic-gamemode
ensure hardcap
ensure baseevents
# QBCore & Extra stuff
ensure qb-core
ensure [qb]
ensure [standalone]
ensure [voice]
ensure [defaultmaps]
## Permissions ##
# permission Stuff
# Resources
add_ace resource.qb-core command allow # Allow qb-core to execute commands
# Gods Admin and Staff access
add_ace qbcore.god command allow # Allow all commands
# Inheritance Admin and Staff Power In Server
add_principal qbcore.admin qbcore.mod # Allow admins access to mod commands
#add_principal identifier.{{principalMasterIdentifier}} qbcore.god <- doesn't exist yet, change the generated one below to qbcore.god
#-------------------------------------------Nano Max-----------------------------------------------------------
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
