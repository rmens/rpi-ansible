# rpi-ansible
Ansible configuration for using a Raspberry Pi as narrowcasting screen. It boots a full screen Chrome that can dispay any dynamic content on a webpage. I use it with: https://github.com/rmens/kabelkrant

## How to use:
* Install a clean version of 2018-11-13-raspbian-stretch
* Configure host in ```hosts.inv``` and set ```chrome_url```
* Run ```ansible-playbook playbook.yml -i hosts.inv --ask-pass -e ansible_ssh_port=22```
* After first run, the ssh port is changed to 228. Run it again with ```ansible-playbook playbook.yml -i hosts.inv --ask-pass -e ansible_ssh_port=228```
* Reboot and voila!
