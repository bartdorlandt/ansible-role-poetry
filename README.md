# Poetry
Sets up the poetry environment.

## Own actions
Once installed you are responsible for adding the poetry paths to your PATH environment.

    export PATH="$HOME/.local/bin:$PATH"

## Requirements
- python3
- curl

## Role Variables
Available variables are listed below, along with default values (see defaults/main.yml):

    virtualenvs_in_project: false
    virtualenvs_prefer_active_python: false
    poetry_ohmyzsh_plugin: false

The top two are setting poetry configuration settings. The poetry_ohmyzsh_plugin flag can be used to enable poetry for ohmyzsh.


## Dependencies
If homebrew (MacOS) was used to install poetry, it would not install it again using the 'normal' installer.

## Example Playbook

    - hosts: localhost
      roles:
        - role: bartdorlandt.poetry

or with variables:

    - hosts: localhost
      roles:
        - role: bartdorlandt.poetry
          vars:
            virtualenvs_in_project: true
            virtualenvs_prefer_active_python: true
            poetry_ohmyzsh_plugin: true

## License

MIT/BSD

## Author Information

This role was created in 2022 by Bart Dorlandt.
