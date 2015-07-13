ansible-ohmyzsh
=======================

An [ansible](http://ansible.com) role that install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

Features
--------

- Installs [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh), A community-driven framework for managing your zsh configuration.

Dependency
----------

- [zsh](http://zsh.org) shell.

Install Ansible
---------------

```fish
sudo apt-add-repository -y ppa:ansible/ansible
sudo apt-get update
sudo apt-get install -y ansible
```

Playbook
--------
```yaml
- hosts: all
  roles:
    - ansible-ohmyzsh
```

Running playbook
----------------
###1 clone this repo
```fish
git clone https://github.com/veggiemonk/ansible-ohmyzsh
```

###2 put the playbook at the same level at the repository you just cloned

###3 run playbook
- `ansible-playbook --inventory 'localhost,' -a -u LOCAL_USERNAME playbook.yml`

Make sur you can connect to localhost by ssh.

Authors
-------
- [veggiemonk](https://github.com/veggiemonk)
Based on the work of:
- [Luke Macken](http://lewk.org) ([@lmacken](http://twitter.com/lmacken))

Special Thanks
--------------
- [Adam Brett](https://adamcod.es) for the best and only ansible tutorial you
  will ever need to get started:
  [link](https://adamcod.es/2014/09/23/vagrant-ansible-quickstart-tutorial.html)
