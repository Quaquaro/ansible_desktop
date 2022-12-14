# Setup Manjaro or EndeavourOS

Ansible playbooks for Manjaro and EndeavourOS

## Prerequisites

- Fresh installation of Manjaro or EndeavourOS
- Python
- Ansible
- SSH-Connection for GitLabServer
- Setup Git Server 
- Clone Repository



### Manjaro 
- Install Manjaro 
    - Choose a language, location and keyboard
    - If you want to install EndeavourOS next to Windows choose "Manual partitioning" otherwise choose "Erase disk"
    - Check Encrypt system and set a passphrase
    - Create your user account
    - Hit install! :rocket:
    - Shutdown the system after the installation process is complete
    - Remove the USB-Stick

### EndeavourOS
- Install Endeavour with your preferred desktop environment
    - Choose Online after the start of the install process
    - Choose a language, location and keyboard
    - If you want to install EndeavourOS next to Windows choose "Manual partitioning" otherwise choose "Erase disk"
    - Check Encrypt system and set a passphrase
    - Choose your favorite desktop
    - Leave the default settings for the packages
    - Create your user account
    - Hit install! :rocket:
    - Shutdown the system after the installation process is complete
    - Remove the USB-Stick

## Usage
- After system you have restarted the system
    - Install Ansible:
    - `sudo pacman -S ansible`
    - Eventually connect to VPN
    - Connect to GitLab-Server via SSH
    - Navigate to GitLab and clone the repo
    - `cd ansible_desktop`
    - `ansible-galaxy collection install -r requirements.yml`
    - `ansible-playbook local.yml` 
## TODO
 - Cleaning up and Testing on both Manjaro and EndeavourOS

