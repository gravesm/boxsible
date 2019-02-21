========
boxsible
========

Ultimately, we will manage ansible through pipx, but we need to do some bootstrapping first:

1. install git
2. clone this repo
3. python -m venv temp
4. source temp/bin/activate
5. pip install ansible
6. ansible-playbook -i hosts bootstrap.yml
7. deactivate
8. rm -rf temp

The bootstrap playbook will install a recent python version to .local/bin, install pipx and then use pipx to install ansible.
