# Libraries.io Infrastructure

All the code and configuration for managing the servers that https://libraries.io runs on

## Setup

You'll need Ansible installed to run the playbooks, instructions here: http://docs.ansible.com/intro_installation.html

## Install required roles from Ansible Galaxy

    ansible-galaxy install -r ansible/requirements.yml

## Running playbooks

### main app

For deploying [Libraries.io](https://github.com/librariesio/libraries.io)

    ansible-playbook ansible/main-app.yml -i ansible/inventories/main-app

### Note on Patches/Pull Requests

 * Fork the project.
 * Make your feature addition or bug fix.
 * Add tests for it. This is important so we don't break it in a future version unintentionally.
 * Send a pull request. Bonus points for topic branches.

### Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## Copyright

Copyright (c) 2016 Andrew Nesbitt. See [LICENSE](https://github.com/librariesio/infrastructure/blob/master/LICENSE.txt) for details.
