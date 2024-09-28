NEO5 NVMe
=========

Installs the NEO5 NVMe driver for Raspberry Pi.

Requirements
------------

The Anrgon 40 NEO5 NVMe case is required to use this driver.

Role Variables
--------------

None need to be passed in.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

In the group or host vars file, set the variable `enable_neo5_nvme` to `true` to enable the role. Call the role as a task in the playbook as shown below:

```yaml
    - name: Run role NEO5_NVMe, if enabled
      ansible.builtin.include_role:
        name: NEO5_NVMe
      when: enable_neo5_nvme | default(false)
```

License
-------

BSD

Author Information
------------------

Bluepants.dev
