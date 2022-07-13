# dev-env-setup
Here is my port of my Arch setup to be ran on a remote server running Arch Linux

## Prerequisites
This is ment to be ran locally on a fresh Arch install and ran as root 

## Running 
First, sync mirrors and install Ansible and other utilities:
```pacman -Syy python-passlib ansible git```

Second, install and update the submodules:
```git submodule init && git submodule update```

Run the playbook as root
```ansible-playbook -i localhost playbook.yml```
