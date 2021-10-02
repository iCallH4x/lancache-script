# lancache-script
Script that automatically installs and sets up lancache on Ubuntu 20.04 Linux

This script is designed to be run on a fresh install of ubuntu 20.04, if you already installed docker it has a chance of breaking.

When you run this script, it will first verify you are using Ubuntu 20.04, then it will verify if you are running it with Root Privileges

Markup : *It will run the normal system updates
*It will add the docker repo to the repository list
*It will then install the latest version of docker and docker-compose
*It will then Clone the lancache git repository into /var/lib/lancache (this is default and can be changed at the top of the script)
*It will then set up Auto Restarting for the services, restarting at 3am local system time to update DNS info, and it will restart with the system
*It then starts lancache and activates the auto restart script

The cache directory is by default /var/lib/lancache/lancache
You can change the cache folder during the setup, when configuring the .env

Just set the IP Address as the same IP Address as the machine, if you want extra IP Addresses, you have to set that up prior.
It's the same as manually installing it, though you just do it through a script, you shouldn't have to fear lack of customizability

If there are problems you can open an issue, if you suggest changes feel free to do a pull request. Happy to apply better code
If I don't respond in a timely manner you join my discord server to contact me
https://discord.plexusmc.net
