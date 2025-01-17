# ans_vars_terminal_colors

Define a set of terminal text, background, and cursor colors.

[![Release](https://img.shields.io/github/release/digimokan/ans_vars_terminal_colors.svg?label=release)](https://github.com/digimokan/ans_vars_terminal_colors/releases/latest "Latest Release Notes")
[![License](https://img.shields.io/badge/license-MIT-blue.svg?label=license)](LICENSE.md "Project License")

## Table Of Contents

* [Quick Start](#quick-start)
    * [Use From Playbook](#use-from-playbook)
* [Role Vars](#role-vars)
* [Contributing](#contributing)

## Quick Start

### Use From Playbook

1. Create `requirements.yml` in ansible project root, and add this content:

   ```yaml
   # requirements.yml
   - src: https://github.com/digimokan/ans_vars_terminal_colors
   ```

2. From the project root directory, install/download the role:

   ```shell
   $ ansible-galaxy install --role-file requirements.yml --roles-path ./roles --force-with-deps
   ```

   * _NOTE:_ `--force-with-deps` _ensures subsequent calls download updates_

3. Include the role, with `public: true`, from the project playbook:

   ```yaml
   # playbook.yml
   - hosts: localhost
     connection: local
     tasks:
       - name: "Define a set of terminal text, background, and cursor colors"
         ansible.builtin.include_role:
           name: ans_vars_terminal_colors
           public: true
   ```

## Role Vars

See the role `vars` files:

  * [vars](../vars/main/)

## Contributing

* Feel free to report a bug or propose a feature by opening a new
  [Issue](https://github.com/digimokan/ans_vars_terminal_colors/issues).
* Follow the project's [Contributing](CONTRIBUTING.md) guidelines.
* Respect the project's [Code Of Conduct](CODE_OF_CONDUCT.md).

