# Poetry
Sets up the poetry environment

## Requirements
- python3
- curl

## Role Variables
Available variables are listed below, along with default values (see defaults/main.yml):

    virtualenvs_inproject: true
    virtualenvs_prefer_active_python: true
    poetry_ohmyzsh_plugin: false

The top two are setting poetry configruation settings. The poetry_ohmyzsh_plugin flag can be used to enable poetry for ohmyzsh.


## Dependencies
None

## Example Playbook

    - hosts: localhost
      roles:
        - role: bartdorlandt.poetry

or with variables:

    - hosts: localhost
      roles:
        - role: bartdorlandt.poetry
          vars:
            virtualenvs_inproject: true
            virtualenvs_prefer_active_python: true
            poetry_ohmyzsh_plugin: true



## License

MIT/BSD

## Author Information

This role was created in 2022 by Bart Dorlandt.