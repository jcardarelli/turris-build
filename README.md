# turris-build
Use Ansible to build Turris OS

## Use a virtualenv, don't be an animal
### Create ansible virtualenv
```
virtualenv -p python3 $HOME/.virtualenvs/ansible
```
### Source the virtualenv activate script
```
source $HOME/.virtualenvs/ansible/bin/activate
```
### Install ansible in the virtualenv
```
pip install ansible
```


## Run the playbook
```
ansible-playbook playbook.yml --ask-become-pass
```

`--ask-become-pass` is required to install system packages with apt.
