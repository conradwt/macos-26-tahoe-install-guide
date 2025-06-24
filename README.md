# macOS Tahoe Install Guide

This is a good way to install macOS 26 Tahoe without overwriting your existing macOS version. 
Also, all of the volumes within a container share the available space of the container’s disk.

## Create Volume
 
  - Open Disk Utility app
  - Click View -> Show All Devices
  - In the left sidebar, Select Existing Disk Container
  - Above the Volume, click `+`
  - Enter a Name: `macOS 26`
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

## macOS Sequoia Setup

  - Disable macOS Tahoe 26 Developer Beta
    - Select System Settings -> General -> Software Update -> Beta Updates -> Off
  - Exclude the volume that you used to install `macOS 26 Tahoe`
    - Select System Settings -> Spotlight -> Search Privacy
    - Click the plus button
    - Choose the `macOS 26` volume, and this should appear within the left sidebar of the Finder
    - Click `Done`
   
    Note:  This process is necessary to prevent Spotlight from indexing files, folders, and other information
           from other volumes.
        
## Install

  - Navigate to the installer within `/Applications` folder.
  - Double click to start the installation process, but select the `macOS 26` volume.
  
    Note:  I didn't copy my settings from macOS Sequoia during the installation process.

## macOS 26 Tahoe Post Install

  - Enable macOS Tahoe 26 Developer Beta
    - Select System Settings -> General -> Software Update -> Beta Updates -> macOS Tahoe 26 Developer Beta
  - Exclude `Macintosh HD` volumes
    - Select System Settings -> Spotlight -> Search Privacy
    - Click the plus button
    - Choose the `Macintosh HD`, and this should appear within the left sidebar of the Finder
    - Click `Done`
   
    Note:  This process is necessary to prevent Spotlight from indexing files, folders, and other information
           from other volumes.
  
## Dual Boot
  
  - https://www.youtube.com/watch?v=xzUPFeat9U4
