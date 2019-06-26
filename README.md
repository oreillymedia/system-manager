# Yet Another Ansible System Manager

This project is just designed to be a collection of roles and/or playbooks to
bootstrap and manager a developer machine.

## Setup

The only thing you need to get started using this is a supported OS and Git+Ansible.

If you re not explicitly using a supported OS, but you are using a favor based
on that OS (Manjaro instead of Arch or Mint instead of Ubuntu), everything may still
work. It is certainly worth a try. If it does not, PRs are always welcome to add support
for your preferred distro as long as you do not break any of the existing ones.

### Arch

```bash
$ sudo pacman -S ansible git
```

### Ubuntu

```bash
$ sudo apt install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt update
```
