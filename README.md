# ansible-mongodb
Ansible role for mongodb container

Create `./library` directory in your ansible project:

```
mkdir ./library
```

And configure `ansible.cfg`:

```
[defaults]
roles_path = ./library
```

Add submodule:

```
git submodule add git@github.com:kressh/ansible-mongodb.git library/mongodb
```

See `defaults/main.yml`

Use role:

```yaml
---
- hosts: yourserver.io
  remote_user: ansible
  become: true
  roles:
    - mongodb
```
