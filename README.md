# Test Environment for DevOps Work

This repo contains stuff needed to get a test environment
for trying out devops related things up and running.

## Vagrant

### Installing vagrant

Download [vagrant](https://www.vagrantup.com/downloads.html) and install using the procedures appropriate for your OS.

Make sure you have VirtualBox or a similar hypervisor installed.

### Bring up vagrant boxes

```bash
vagrant up
```

## Saltstack

### Connect minions to master

First, ssh into the salt-master:

```bash
vagrant ssh salt-master
```

Then, discover all minions by using:

```bash
sudo salt-key --list-all
```

Then, accept the minions by using:

```bash
sudo salt-key --accept-all
```