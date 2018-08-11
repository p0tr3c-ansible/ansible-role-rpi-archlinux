# Ansible Role: arch-on-rpi

Install Arch Linux on RPi
## Requirements

Some operations requires root permissions, for example partition sd card.

## Role Variables

All role variables are listed in vars/main.yml.

## Dependencies

None

## Example Playbook

Run with --ask-become-pass

    - hosts: localhost
      connection: local
      tasks:
        - include_role:
            name: ansible-role-rpi-archlinux
          vars:
            sd_card_device_path: /dev/mmcblk0

## License

MIT / BSD
