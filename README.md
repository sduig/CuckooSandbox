# CuckooSandbox
Setup of Cuckoo Sandbox on Ubuntu 16.04 using Windows 7 Image

#Install guide used
https://gist.github.com/braimee/bf570a62f53f71bad1906c6e072ce993

#If the install fails ensure to run these commands before running again
sudo rm -r /home/cuckoo/VirtualBox\ VMs/vm
sudo apt-get remove virtualbox-* --purge -y
VBoxManage hostonlyif remove vboxnet0
VBoxManage hostonlyif remove vboxnet1
sudo reboot

#Remove the cuckoo user created during the install script

#If pip python packages don't install then run the following
sudo wget https://bootstrap.pypa.io/pip/2.7/get-pip.py
python get-pip.py
sudo -H pip install --upgrade pip
pip install --upgrade setuptools
sudo -H python2.7 -m pip install --upgrade pip==20.3.4
sudo reboot



