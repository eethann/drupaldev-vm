#Install

- Install Ansible on your local machine `sudo pip install ansible` (note: brew install doesn't work at the moment)
- Run `ansible-galaxy install -r provisioning/requirements.txt --force`
- Run `vagrant plugin install vagrant-cachier`

#Includes
- PHP 5.5
- Mariadb
- Solr 4.x
- Nginx

#SSH Forwarding

1. Add the following to your .ssh/config:

    `Host 33.33.33.10`

    `AgentForward yes`

2. Run `ssh-add`
3. To test `vagrant ssh` then `ssh -T git@github.com`

#VHOST Config
See `provisioning/vars/example.yml`
