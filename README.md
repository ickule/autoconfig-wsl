# Autoconfig WSL

This repository will hold my personal configs for the autoconfigurating my Ubuntu using Ansible.
it can be used on any Ubuntu based system.
(yes, this is a fancy overkill dotfile kinda repo.)

It mainly install zsh, with syntax highlighting, auto-suggestions, auto-completion and powerlevel10k prompt.

## 1. Requirements

### 1.1 Ansible

Install ansible with the following:

```bash
sudo apt install -y ansible
```

## 1.2 Set user as passwordless sudo

Edit your sudoers file with and edit the line 50 to add passwordless sudo access to sudo group.

```sh
sudo visudo
change this -> %sudo   ALL=(ALL:ALL) NOPASSWD: ALL
```

## 2. Using the ansible playbook

With a system featuring the previous requirements, we can run the playbooks.

```bash
ansible-playbook autoconfig-wsl.yml
```

## Credits/Sources
