# CuckooSandbox
Setup of Cuckoo Sandbox on Ubuntu 16.04 using Windows 7 Image

#Install guide used
https://gist.github.com/braimee/bf570a62f53f71bad1906c6e072ce993

#If the install fails ensure to run these commands before running again:

1. sudo rm -r /home/cuckoo/VirtualBox\ VMs/vm
2. sudo apt-get remove virtualbox-* --purge -y
3. VBoxManage hostonlyif remove vboxnet0
4. VBoxManage hostonlyif remove vboxnet1
5. sudo reboot

#Remove the cuckoo user created during the install script

#If pip python packages don't install then run the following:

1. sudo wget https://bootstrap.pypa.io/pip/2.7/get-pip.py
2. python get-pip.py
3. sudo -H pip install --upgrade pip
4. pip install --upgrade setuptools
5. sudo -H python2.7 -m pip install --upgrade pip==20.3.4
6. sudo reboot



