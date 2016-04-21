# first install Ansible doing the following steps

sudo apt-get install software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible python-pip git
sudo pip install clc-idk requests --upgrade
# Export your CLC credentials before running the ansible-playbook build command

export CLC_V2_API_USERNAME=CLC_USER
export CLC_V2_API_PASSWD=‘CLC_PASSWORD'
export CLC_SERVER_PASSWORD=’SERVER_PASSWORD’


# graylog

When using the build.yml make sure to change the (CHANGE OPTIONS TO FIT YOUR NEED) 

ansible-playbook -i clc_inv.py build_gray.yml
