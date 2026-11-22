###### 11/22/2026 ######
Today I am attempting to categorize my homelab machines and home network devices into different groups on my network.  I am looking to put home devices on 192.168.0.x, homelab experimental devices on 192.168.20.x, and homelab production devices on 192.168.30.x.

In Proxmox, I created a new network Linux bridge, and will be creating a new VM with OPNsense running on it.

I set up an Ubuntu desktop for GUI configuration of OPNsense and to verify it was working.  I encountered an issue when trying to connect through the OPNsense router.  It turned out that the ipv4 connection method was set to auto instead of manual, which was causing trouble during static address testing.