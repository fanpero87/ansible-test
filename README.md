# Ansible Automation

This repo allows you to use "ansible-pull" to automate some tasks.

## Install Ansible

In order to use this method, you need to install ansible on the machine you want to run this. On an Ubuntu or Debian distro just run:

```sh
apt install ansible -y
```

## Run Ansible

Now that Ansible is installed, just run:

```sh
sudo ansible-pull -U https://github.com/fanpero87/ansible-test.git
```

### What's doing

This repo will do:

- Run `apt update` on the server
- Create two users (ansible and dev) and setup their profiles
- Install some packages
- Create a crontask to run the `ansible-pull` command automatically every 10 min if there is a change on the repo

### Disclaimer

This repo was made following this [Youtube video](https://youtu.be/sn1HQq_GFNE) and this [Github repo](https://github.com/LearnLinuxTV/personal_ansible_desktop_configs)
