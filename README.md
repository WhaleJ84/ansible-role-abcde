abcde
=========

Installs and configures abcde for the user.

Requirements
------------

To include this role in your `requirements.yml` file, add the following list item:

```yaml
---
roles:
  - name: whalej84.abcde
    src: https://github.com/WhaleJ84/ansible-role-abcde.git
    scm: git
```

Role Variables
--------------

| Name | Type | Description | Default |
| ---- | ---- | ----------- | ------- |
| abcde\_config | string | A filepath to the abcde configuration file. | $HOME/.abcde.conf |
| abcde\_vars |  |  | None |

Example Playbook
----------------

This example playbook shows how I would use this role, with custom variables to suit my needs.

```yaml
---
- hosts: localhost

  roles:
    role: whalej84.abcde
    tags: [ abcde ]
```

