# Sandstorm Ansible Installation

For a description of the background of this project, see https://sandstorm.de/de/blog/ansible-mac-os-x.html


## Prerequisite: XCode

* Make sure you have XCode installed
* Make sure you have XCode command line tools installed


## Cloning Ansible-OSX

If you are reading this file on your local machine, you have already done this step:

```
git clone https://github.com/knomic/macosx-with-ansible.git ~/sandstorm-ansible
```


## Installation

Installs Ansible and Homebrew.

```
cd ~/sandstorm-ansible
# make sure that [username].yml exists
cat ${USER}.yml

./boot.sh
```


## Initial Run

Now, do the following steps for the initial setup:

* make sure to open a *fresh Terminal window*
* `./run.sh` -- this will *FAIL* at the "compass" installation
* *CLOSE* the terminal-window and re-open another one.
* `./run.sh` -- this should now run through


## Running (to apply changes)

```
./run.sh
```


## Development Helpers (not needed for normal people)

```
./run.sh --skip-tags=slow
./run-nosudo.sh
```

## Learning Ansible / References

* See http://docs.ansible.com/playbooks_intro.html for the ansible documentation
* Templates: http://jinja.pocoo.org/docs/templates/
* Install npm-packages: http://docs.ansible.com/npm_module.html

