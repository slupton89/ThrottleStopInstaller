# ThrottleStopInstaller
Installs Throttlestop and adds and entry to the registry to start with windows. No more dealing with UAC, creating tasks, or only having the program launch in the background.

Check releases for the latest version of the installer. To build or update yourself see below.

## Updating

Clone this repo and download latest version of Throttlestop from https://www.techpowerup.com/download/techpowerup-throttlestop/

Place the extracted files in the CurrentVersion folder
* Don't overwrite Throttlestop.ini - This is setting defaults to prevent from running in background only
* New files that may be added in new versions will also need to be linked in the [Files] section of the SetupScript.iss

Build SetupScript.iss with InnoSetupCompiler

## Advanced

* If you want to create a preconfigured build for reinstall only - replace the included Throttlestop.ini with your pre-existing ini(This isn't advised for installing on pc's that the ini wasn't configured for as the voltages may not work with the CPU)
