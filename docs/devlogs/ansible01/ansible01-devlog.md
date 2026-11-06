###### 11/1/2026 ######
Tonight, I entered the public SSH key into Github for this repo.
- Completed SSH into web01
- Created playbook, inventory, and config file for ansible.  Verified operational with an all-machine ping test, returning pong.

###### 11/5/2026 ######
I deployed nginx to web01 device, and verified that the html document was accessible via the curl command, as well as manually verifying through my PC browser.  I made some changes to the index.html document on the web01 device, then was able to overwrite and reconfigure using another playbook push through ansible.