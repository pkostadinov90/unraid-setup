# unraid-setup
Personal notes on setting up Unraid server

# Installation

## Tools
 - Apps store plugin
 - Dev Pack plugin
 - Nerd Pack plugin

Docker:
 - DockerHub:	plexinc/pms-docker

VMs:
 - Windows 10
   - Video driver from the disk to enable more than 800x600
   - Network bridge: br0
   - Setup home Router for static IP
   - Enable RD inside the VM
   
## Big Fails
 - No decent torrent client found, so installed Windows 10 VM just for the uTorrent with some RD and TeamViewer backup

# Migration

## Plex

Resources:

Migrate libraries - this is not really needed, we could simply re-scan folders, and be running eventually:
 - https://support.plex.tv/articles/201370363-move-an-install-to-another-system/

Migrate Watched Status:
 - https://support.plex.tv/articles/201154527-move-viewstate-ratings-from-one-install-to-another/1579390663
 - https://forums.plex.tv/t/importing-view-state-ratings-from-db-files/58880/9 - if the import is messed up, this will empty the database with watched statuses
 - https://forums.plex.tv/t/how-to-transfer-plex-library-from-windows-to-linux/90633 - some stored article, that may be of some use, just backing a tab

Home Screen Reset - upon too many changes, home sceren stops working properly, this will reset to original state:
 - https://support.plex.tv/articles/customizing-plex-web/
 

# TO DO:
 - Figure out how to Backup FlashDrive containing unRaid
 - Figure out how to back appdata or at least:
   - Plex Folder
   - uTorrent Folder from within WindowsVM
 - Expose PlexServer to the router for outside access
 - Expose Windows RD to the router for outside access
 - Map a subdomain to router real IP
