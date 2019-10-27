# Innovation-Games-Ansible
The entirety of the Innovation Games server deployment is being build using Ansible Playbooks in order to allow us to better scale our server solution. This repository contains everything you would need in order to start building your own version of The Innovation Games should you wish to do so. 

## Inventory Files
In order to ensure we are able to protect the core infrastructure appropriately, we do not include our inventory files within this project, however there are placeholder files in place which you can modify yourself. 

## Requirements File
In order to download the required roles, you will need to run `ansible-galaxy install -r requirements.yml` to download the roles. 

## Known Issues
An issue has been identified where the yum module seems to hang on first load, this can often make it easier to just update by hand on the boxes as you provision them, as you currently have to login anyway to add the SSH Key to your known hosts. 