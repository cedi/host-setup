# localhost setup

this ansible playbook does the basic setup of my local machine.

## Contents

This will install some basic software, required for my development workflow, as well as a local prometheus server and a grafana, so I can monitor my system a little better ;-)

## Setup

```
git submodule init
git submodule update --recursive
```

## Run

```
ansible-playbook setup.yml --inventory=inventory.yml --ask-become-pass
```
