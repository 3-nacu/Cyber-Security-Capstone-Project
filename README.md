# Cyber-Security-Capstone-Project

Welcome to my Cyber Security Capstone, in this project I will demonstrate how to create a VLAN infrastructure in which we will set up services
in a segemented part of the network. We will also create a subnet where our "Users" will be located, and they will be able to interact within the VLAN and to 
the Internet. Once all set up is complete we will test default configurations and perform a penetartion test in order to see how we will harden our sytems.

In order to get started we have to begin with configuring our managed Cisco switch. Lets firstly create a VLAN ID number and then we will configure more settings 
like the distributed port group to match our recently created VLAN ID in our cluster of ESXis VMware servers.

In your managed switchs terminal type:
# sh int status | i connected

This will prompt you to all the connected interafaces in your swtich, in here you want to configure trunking if you have not already, this will enable cross communication between all your VLANS.

If you don't have a VLAN created you can do so by typing:
# vlan 123
Followed up by another command that specifies your preferred name:
# name my_first_vlan
Then end the configuration and save for next startups:
# end
# wr me
# copy running-config startup-config
# exit 





