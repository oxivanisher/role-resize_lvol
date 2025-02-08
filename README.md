resize_lvol
===========

Resize a LVM logical volume.
The default value of the size is resizing the LV to the complete free space in the PV.

Role Variables
--------------

| Name             | Comment                              | Default value                   |
|------------------|--------------------------------------|---------------------------------|
| resize_lvol_lv   | The LV name to be resized.           | `` |
| resize_lvol_vg   | The VG name of the lV to be resized. | `` |
| resize_lvol_size | The target size of the LV.           | `100%PVS` |


Example Playbook
----------------
```yaml
- name: Resize LV
  hosts: all
  collections:
    - oxivanisher.linux_base
  roles:
    - role: oxivanisher.linux_base.resize_lvol
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_base](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_base/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_base).
