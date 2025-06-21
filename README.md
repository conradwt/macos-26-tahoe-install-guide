# macOS Tahoe Install Guide

## Create Volume
 
  - Open Disk Utility app
  - Click View -> Show All Devices
  - In the left sidebar, Select Existing Disk Container
  - Above the Volume, click `+`
  - Enter a `Name:`
  - Click `Add`
  
  Note: https://www.youtube.com/watch?v=vk1xK28KkLA
  
## Download Installer
  
  - Option #1
  
    - select System Settings -> General -> Software Update -> Beta Updates -> macOS Tahoe 26 Developer Beta
    - From the Terminal, type the following:
    
      ```zsh
      softwareupdate —list-full-installers
      softwareupdate —fetch-full-installer —full-installer-version 26.0
      ```

    Note: https://www.youtube.com/watch?v=EVeQrk4MyB0 
    
  - Option #2 - If the Option #1 doesn’t work, download the installer from the following location:
  
    - https://mrmacintosh.com/macos-tahoe-full-installer-database-download-directly-from-apple

## Cleanup

  - In the current macOS version, do the following:
  
    - select System Settings -> General -> Software Update -> Beta Updates -> Off
  
## Install

  - Locate the installer with /Applications folder
  - Double click to start the installation process
  
  Note:  I didn't copy my settings from macOS Sequoia during the installation process.
  
## Dual Boot
  
  - https://www.youtube.com/watch?v=xzUPFeat9U4
  
Notes:  

- This is a good way to install macOS 26 Tahoe without overwriting your existing macOS version. 
  Also, all of the volumes within a container share the available space of the container’s disk.
  
