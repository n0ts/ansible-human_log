# ansible-human_log

This Ansible callback plugin for human-readable result logging for Ansible 2.0-2.4.
It [used to support 1.9.x](https://github.com/n0ts/ansible-human_log/issues/15),
but this is not the case any more.

## Usage

To use, set the callback plugins directory in ansible.cfg:
```
[defaults]
callback_plugins = path/to/callback_plugins/
```

## Debug

To debug, set in ansible.cfg:
```
[defaults]
stdout_callback = debug
```

or define environment variable `ANSIBLE_STDOUT_CALLBACK = debug'


## Reference

Inspired from: https://github.com/redhat-openstack/khaleesi/blob/master/plugins/callbacks/human_log.py
Original from: https://gist.github.com/cliffano/9868180
