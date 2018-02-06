# ansible-human_log

This Ansible callback plugin for human-readable result logging for Ansible 2.0-2.4.
It [used to support 1.9.x](https://github.com/n0ts/ansible-human_log/issues/15),
but this is not the case any more.  Also it is of limited use for 2.2 onwards,
as explained in the Alternative section below.

## Usage

To use, set the callback plugins directory in ansible.cfg:

```
[defaults]
callback_plugins = path/to/callback_plugins/
```

## Alternative

Ansible 2.2
[introduced](https://github.com/ansible/ansible/commit/d2438b6b6b9dbb5f0f320fbe9e6e30b102006c1d)
the [`debug` output callback](http://docs.ansible.com/ansible/devel/plugins/callback/debug.html)
which offers very similar functionality to this `human_log` callback.

To use the `debug` callback, set the following in `ansible.cfg`:

```
[defaults]
stdout_callback = debug
```

Alternatively you can set the environment variable
`ANSIBLE_STDOUT_CALLBACK` to `debug`.


## Reference

Inspired from: https://github.com/redhat-openstack/khaleesi/blob/master/plugins/callbacks/human_log.py
Original from: https://gist.github.com/cliffano/9868180
