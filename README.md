# Sysctl automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-sysctl
  name: ansible-role-sysctl
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-sysctl

- Import role and override role variables, e.g.
```
- name: Setup sysctl
  roles:
    - role: ansible-role-sysctl
```

- All available role vars can be found in `defaults`
