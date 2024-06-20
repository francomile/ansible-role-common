# Ansible Common Role

[![Lint Ansible roles](https://github.com/francomile/ansible-role-common/actions/workflows/ansible_lint.yml/badge.svg)](https://github.com/francomile/ansible-role-common/actions/workflows/ansible_lint.yml)

[![Release role to Ansible Galaxy](https://github.com/francomile/ansible-role-common/actions/workflows/push_to_galaxy.yml/badge.svg)](https://github.com/francomile/ansible-role-common/actions/workflows/push_to_galaxy.yml)

## Actions of the Role

* Update all packages to the latest version
* Install common packages
* Remove insecure legacy packages
* Set Timezone
* Set limits.conf
* Update `journald.conf`
* Update rsyslog logrotate
* Set vm.swappiness default

## Common Usage

```yaml
roles:
  - {
    role: francomile.common,
    tags: ["common"]
    }
```

## Run the playbook

```shell
ansible-playbook -i inventory playbook.yaml --tags "common"
```
