# Ansible Linux Mint Post-Installation (localhost)

Ansible playbook for installing tools and applications on localhost with Linux Mint Cinnamon Edition.

## Linux Mint Releases

https://linuxmint.com/download.php

## Linux Mint Installation (manual steps)

1. Start _Install Linux Mint_
1. _English_
1. _English (US)_ - _English (US)_
1. _Install multimedia codecs_
1. _Erase disk_ (_LVM_ + _Encrypt_)
1. `<Your_City>`
1. _Your name:_ `<Firstname>` `<Lastname>`
1. _Your computer's name:_ `<Your_PC_Name>`
1. _Pick a username:_ `<Your_Username>`
1. _Require login_

## System Settings and Preparations

### Virtualbox Guest Additions Installation (optional)

    $ sudo apt update
    $ sudo apt upgrade
    $ sudo apt install build-essential module-assistant
    $ sudo m-a prepare

Choose in VirtualBox window menu bar: _Devices > Insert Guest Additions CD image_

### Ansible installation

    $ sudo apt update
    $ sudo apt install software-properties-common
    $ sudo add-apt-repository --yes ppa:ansible/ansible
    $ sudo apt install ansible


## Usage

    ansible-playbook site.yml --K
