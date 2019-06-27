# Yet Another Ansible System Manager

This project is just designed to be a collection of roles and/or playbooks to
bootstrap and manager a developer machine.

## Requirements

The only thing you need to get started using this is a supported OS and
Git+Ansible.

If you re not explicitly using a supported OS, but you are using a favor based
on that OS (Manjaro instead of Arch or Mint instead of Ubuntu), everything may
still work. It is certainly worth a try. If it does not, PRs are always
welcome to add support for your preferred distro as long as you do not break
any of the existing ones.

### Arch Requirements

```bash
$ sudo pacman -S ansible git
```

### Ubuntu Requirements

Tested against Ubuntu 19.04

```bash
$ sudo apt install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt update
$ sudo apt install ansible git
```

## Setup

## Changing Display Managers

When you want to change your default display manager, it takes a bit of extra
effort to switch them.

### Arch Display Manager

```bash
$ sudo systemctl stop display-manager
$ sudo systemctl disable display-manager
```

Update `desktop_display_manager` in your `user.yml` and then the new display
manager will be enabled.
