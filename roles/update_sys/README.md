# update_sys

_An ansible role to:_ Update all the systems!

## Usage

Include in a playbook with the following:

```yaml
- hosts: localhost

  roles:
    - { role: bluepantsdev.update_sys }
```

## Variables

`update_sys_enabled` - Whether or not to run the role. Default is `true`.

`apt_upgrade` - For apt systems, select the type of upgrade to run. Default is `dist`.

## Dependencies

None

## License

TBD

## Author

Created in 2024 by shaunsund. See more of my work at [https://bluepants.dev](https://bluepants.dev).