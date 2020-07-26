# MyLucie machine

A machine that runs services to support MyLucie, a photo and video company, to sharing files with team members

## Machine requirements

A CentOS 8 machine with sufficient space in /var/www/html and some user that can connect to it. (See `group_vars/all/bootstrap.yml` which refers to `group_vars/vault.yml` for a username.)

## One time setup

```
ansible-galaxy install -r roles/requirements.yml -f
```

## Install

```
ansible-playbook -K playbook.yml
```
