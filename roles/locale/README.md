# locale

Sets the system locale.

## Requirements

- Ansible 2.9 or later
- Python 3.6 or later

## Role Variables

The following variables can be set to configure the motd:

- `LOCALE` - Set to the desired locale. Default is `en_US.UTF-8`.

## Role Operation

We change the file `/proc/device-tree/model` to see if a machine is a Raspberry Pi. We then check `/etc/default/locale` to see if the locale is already set. If it is not, we set the locale to the value of the `LOCALE` variable using the `raspi-config nonint do_change_locale` command.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - name: Set Raspberry Pi localization to US
      role: bluepantsdev.raspberrypi.locale
```

## License

MIT
