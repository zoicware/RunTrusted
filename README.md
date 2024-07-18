## Run Trusted

#### How it Works

Gaining TrustedInstaller privileges can be done multiple ways but all methods require the use of the TrustedInstaller service in windows. This function exploits the binary path of this service to run powershell commands instead of the default TrustedInstaller.exe [Read More](https://www.tiraniddo.dev/2017/08/the-art-of-becoming-trustedinstaller.html)

#### Features

- Run any powershell commands silently 

- Pass commands that contain spaces in the path without issues
    - all commands are ran as Base64 strings to escape these spaces

##### Tip: to troubleshoot errors redirect the error to a txt doc using the built in $Error variable in PowerShell