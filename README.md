# ansible-shelly
ansible framework to install Allterco Robotics shelly devices on your network

you can configure all of your local or remote shelly devices gen1 and gen2.

* installation:
 cd ansible-shelly
 # clone this repository
 git clone https://github.com/elbrondor/ansible-shelly.git
 # create your secrets:
 echo "some chars as you want for encryption" > .vault_password_file
 cp group_vars/all/secrets.yml.example group_vars/all/secrets.yml
 ansible-vault encrypt group_vars/all/secrets.yml
 
 # for eatch shelly you can create it's own defaults see examples in host_vars/
 # but keep in mind to copy all settings from the default. Current it's not possible
 # to overwrite one item.
