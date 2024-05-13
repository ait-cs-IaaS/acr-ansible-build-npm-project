# Ansible-Role: acr-ansible-build-npm-project

AIT-CyberRange: Builds npm project and copies it to a live directory.


## Requirements

- Debian or Ubuntu 

## Role Variables

```yaml
project_user: username
project_path: /project
project_env: {}
project_dest: /var/www/html/project
```

## Example Playbook

```yaml
- hosts: all
  roles:
    - acr-ansible-build-npm-project
      vars:
        project_user: "{{ appname_user }}"
        project_path: "{{ appname_basepath }}/frontend"
        project_env: "{{ appname_env }}"
        project_dest: /var/www/html/appname
```

## License

GPL-3.0

## Author

- Lenhard Reuter