# Kafka-End-to-End-Pipeline-phase1

## Main steps
* create redhat account as we are going to use redhat linux for development
* After logged into redhat, click okay on T&C.
* Then go to developer tools section, and then install redhat enterprise linux image.
* In local system install VM Ware or VM box for using redhat OS without disturbing the our original OS.
* While installing the RHEL on VMware it will ask about basic options, like creating root user, normal user, ram, disc space, location and
  for software it will ask regarding basic environment and add ons.
* Pick minimal install while installing rhel on vm.

### Once logged into new VM, run below commands
With only 2GB RAM, swap space can help avoid memory-related crashes.
Create a 2GB swap file
* Enable Swap Space
* 
sudo fallocate -l 2G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile
echo '/swapfile swap swap defaults 0 0' | sudo tee -a /etc/fstab

 Install Networking and Essential Tools

 sudo yum install wget curl net-tools -y

 

