# ansible-nodejs

Simple role to facilitate installing node with nave.

## Configuration

Only one variable `nodejs_version` is used.

## When node updates

You can detect if node was reinstalled using `nodejs_version_installed|changed`

## Usage:

```yaml
# playbook.yml
- name: "Node"
  become: yes
  become_user: root

  vars:
    nodejs_version: 4.1.1

  roles:
    - nodejs
```
