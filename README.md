# PixelBuilds-build-signed-script
Script for creating a signing build environment

## Disclaimer
This script only works for password-less keys (DO NOT SET A PASSWORD) *This is due to building inline, other steps are necessary for a password*

*Works with PixelBuilds Unity*

## How to run
1. Download the script in your root build directory and run it

`wget https://raw.githubusercontent.com/alexismdr/pixelbuilds-build-signed-script/main/create-signed-env.sh`

`chmod +x create-signed-env.sh`

`./create-signed-env.sh`

2. Enter info for certificate subject line and confirm

3. Hit enter to set no password for each certificate. **Cannot set a password to build inline with this method!**

4. In your device tree (or common device tree) add: `-include vendor/pixelbuilds-priv/keys/keys.mk`

5. Build as usual! 
