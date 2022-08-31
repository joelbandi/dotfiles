# Dotfiles and Dev system management with Ansible


This Project contains some configuration and yaml files that allows Ansible to setup my dev environment in a brand new MacOs environment including packages, apps, system config and .*rc files in a consistent and reproducible way to your liking

It uses ansible [core 2.13.3]
 
### Things it does
 - Install Zshell
 - Copy Zshell config and aliases
 - Install asdf
 - Copy the global tool versions
 - Install node
 - Copy Node config
 - Install favorite node packages
 - Install ruby
 - Copy Ruby config
 - Install favorite ruby packages
 - Install Go
 - Configure github

### How to use it.

1. Install `ansible` in your client machine
2. Download this project or clone this project to your machine
3. Check to make sure the variables in `group_vars/local` file in this project has the correct values
4. Run `ansible-playbook -i hosts.yml playbook.yml` to automatically terraform your machine.
5. Customize playbook.yml according to you liking if you need to make any changes or add any steps.

The `Vagrantfile` is just used for testing this playbook.
