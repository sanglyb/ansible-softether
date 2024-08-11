# Ansible Softether
## What is it
Ansible playbook to quickly deploy [SoftEtherVPN](https://www.softether.org/) to your server. Tested on Ubuntu 24.04 and Ubuntu 20.04. Playbook can install a package from apt, if it persists in repo, if not - it will be compiled from sources. 

## Prerequisites
Install ansible:
```
sudo apt install ansible
```
Add required servers to the hosts file, line by line.
Copy `group_vars/vars.yml.example` to `group_vars/vars.yml` and set your domain, users and passwords. 
Run playbook:
```
ansible-playbook vpn.yml -i hosts
```

If you don't need any steps, for example, let's encrypt certificate, you can comment out required lines in `vpn.yml`.

## Visit my blog for tech articles
My blog - [https://www.mytechnote.ru](https://www.mytechnote.ru)
