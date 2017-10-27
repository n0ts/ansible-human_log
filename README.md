# ansible-human_log

This Ansible callback plugin for human-readable result logging for Ansible 1.9/2.0.

To use, set the callback plugins directory in ansible.cfg:
```
[defaults]
callback_plugins = path/to/callback_plugins/
```

Inspired from: https://github.com/redhat-openstack/khaleesi/blob/master/plugins/callbacks/human_log.py
Original from: https://gist.github.com/cliffano/9868180
