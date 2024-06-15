# Common role

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
    role: common,
    tags: ["common"]
    }
```

## Run the playbook

```shell
ansible-playbook -i inventory playbook.yaml --tags "common"
```
