# localhost setup

this ansible playbook does the basic setup of my local machine.

## Contents

This will install some basic software, required for my development workflow, as well as a local prometheus server and a grafana, so I can monitor my system a little better ;-)

## Setup

```
git submodule init
git submodule update --recursive
```

## Run Ansible

### All

This is usefull for a new host

```
ansible-playbook main.yml --inventory=inventory.yml --ask-become-pass
```

### Setup

This is used if you do changes regarding the installed software, configuration, etc.

```
ansible-playbook setup.yml --inventory=inventory.yml --ask-become-pass
```


### Prometheus

This is used if you do changes to the prometheus setup

```
ansible-playbook prometheus.yml --inventory=inventory.yml --ask-become-pass
```

### Grafana

This is used if you do changes to the grafana setup

```
ansible-playbook grafana.yml --inventory=inventory.yml --ask-become-pass
```


