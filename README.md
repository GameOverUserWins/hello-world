# RiceRobot's Jellyfin Home Media Server 
UPDATE 30 Aug 2023: RiceRobot is back baby. A short hiatus and sabbatical from the world of IT to pick up some much needed edumacation, and now it's time to put the cyber hat back on.
So let's get some brainstorming on the planned build. AKA Documentation, let's goooo.

Planned Build: Network Streaming Home Media Server
Requirements:
  Network media streaming to 1-4 users within LAN.
  Video up to ~1080p @ 60FPS.
  Remote monitoring of local network uptime.
  
Server Hardware
  1U Dell R220 (acquired)
    16GB
    250GB OS drive
    xTB RAID array for hosting media (to be deployed)
    1GB network uplink to local switch

  Server Configuration Architecture
    Proxmox Hypervisor
      Fedora Server
        Physical storage array allocated to Fedora.
        Docker
          JellyFin, with media mounted via storage on fedora host.
          Uptime/heartbeat to upstream/out of LAN monitoring
