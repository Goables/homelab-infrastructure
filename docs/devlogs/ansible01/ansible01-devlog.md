###### 11/1/2026 ######
Tonight, I entered the public SSH key into Github for this repo.
- Completed SSH into web01
- Created playbook, inventory, and config file for ansible.  Verified operational with an all-machine ping test, returning pong.

###### 11/5/2026 ######
I deployed nginx to web01 device, and verified that the html document was accessible via the curl command, as well as manually verifying through my PC browser.  I made some changes to the index.html document on the web01 device, then was able to overwrite and reconfigure using another playbook push through ansible.

###### 11/7/2026 ######
Learning how to use variables in playbooks and package deployments.  Also learning about handlers and templates.  I'm interested to see how you can use dynamic variables for use in multiple machines from one deployment.  For example, having each machine display a webpage through nginx saying "I am machine 02" for machine 02, 03 for machine 03, etc, all with one deployment.  I know it's possible, but that is my current curiosity regarding this.

I deployed the package, but it didn't show up in the hosted webpage.  After looking back at the playbook file, I realized that out of habit I accidentally set the destination for the html file to "index.js" instead of "index.html."  After fixing, the webpage displayed correctly.