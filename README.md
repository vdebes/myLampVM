# My LAMP VM

This is just a Vagrant box with the stack I use on a regular basis. 
Based on debian/jessie, nothing fancy, provisioned with Ansible. 

## Getting started
```
git clone https://github.com/vince-db/myLampVM.git
cd myLampVM
vagrant plugin install vagrant-vbguest
vagrant plugin install vagrant-guest_ansible
vagrant up
```
Then go to [http://192.168.33.10](http://192.168.33.10) and you are good to go. 

## Customize the configuration
Modify playbook.yml, then run
```
vagrant reload --provision
```