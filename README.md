# OpenConnect Pulse TFA script

This script simplifies connecting to PulseVPN servers with Two-Factor-Authentication enabled.

## Requirements
- openconnect
- curl
- oathtool (Optional)

## Usage
1. Create the config file `~/.pulsevpn` with 3 lines:
```
servers=("https://pulse.vpn.site" "https://pulse2.vpn.site")
secrets=("SECRET-SERVER1" "SECRET-SERVER1") (Optional)
username=YOUR-USERNAME
password=YOUR-PASSWORD
```

2. Run the script and insert the OTP when asked.  
(Optionally) You skip the insertion of OTP by configuring your secret in the config file
(Optionally) The script can be called with one argument: `connect_pulse.sh <path_to_config_file>`
